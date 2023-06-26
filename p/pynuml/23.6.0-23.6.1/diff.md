# Comparing `tmp/pynuml-23.6.0.tar.gz` & `tmp/pynuml-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynuml-23.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynuml-23.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynuml-23.6.0.tar` & `pynuml-23.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       17 2022-08-22 18:47:46.562567 pynuml-23.6.0/.gitignore
--rw-r--r--   0        0        0      824 2023-06-15 20:05:13.774670 pynuml-23.6.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1074 2023-05-23 17:23:11.333385 pynuml-23.6.0/LICENSE
--rw-r--r--   0        0        0     5647 2023-05-11 17:09:33.660248 pynuml-23.6.0/README.md
--rw-r--r--   0        0        0      170 2022-08-22 18:47:46.563031 pynuml-23.6.0/doc/README.md
--rw-r--r--   0        0        0     9267 2022-08-22 18:47:46.563254 pynuml-23.6.0/doc/graph_create.md
--rw-r--r--   0        0        0     2903 2022-08-22 18:47:46.563416 pynuml-23.6.0/doc/python_env.md
--rw-r--r--   0        0        0      638 2023-05-23 17:23:11.333546 pynuml-23.6.0/docs/Makefile
--rw-r--r--   0        0        0      923 2023-06-15 20:05:13.774909 pynuml-23.6.0/docs/conf.py
--rw-r--r--   0        0        0      673 2023-06-15 20:05:13.775100 pynuml-23.6.0/docs/index.rst
--rw-r--r--   0        0        0     1413 2023-06-15 20:05:13.775357 pynuml-23.6.0/docs/install/installation.rst
--rw-r--r--   0        0        0      804 2023-05-23 17:23:11.333683 pynuml-23.6.0/docs/make.bat
--rw-r--r--   0        0        0      581 2022-08-22 18:47:46.563608 pynuml-23.6.0/example/plot.py
--rwxr-xr-x   0        0        0     2089 2022-11-30 18:31:20.903706 pynuml-23.6.0/example/process.py
--rw-r--r--   0        0        0     1169 2022-08-22 18:47:46.563858 pynuml-23.6.0/h5merge.py
--rw-r--r--   0        0        0       38 2022-10-01 15:34:05.362452 pynuml-23.6.0/pynuml/.gitignore
--rw-r--r--   0        0        0      164 2023-06-15 20:05:13.776439 pynuml-23.6.0/pynuml/__init__.py
--rw-r--r--   0        0        0       97 2023-02-27 22:44:16.230810 pynuml-23.6.0/pynuml/io/__init__.py
--rw-r--r--   0        0        0    33647 2023-05-23 17:23:11.334552 pynuml-23.6.0/pynuml/io/file.py
--rw-r--r--   0        0        0     3290 2023-05-23 17:23:11.334785 pynuml-23.6.0/pynuml/io/h5interface.py
--rw-r--r--   0        0        0     4089 2023-05-23 17:23:11.334967 pynuml-23.6.0/pynuml/io/out.py
--rw-r--r--   0        0        0      102 2023-06-15 20:05:13.776689 pynuml-23.6.0/pynuml/labels/__init__.py
--rw-r--r--   0        0        0     1476 2022-10-01 15:34:05.363366 pynuml-23.6.0/pynuml/labels/ccqe.py
--rw-r--r--   0        0        0     1156 2023-06-15 20:05:13.776860 pynuml-23.6.0/pynuml/labels/flavor.py
--rw-r--r--   0        0        0      779 2023-05-23 17:23:11.335229 pynuml-23.6.0/pynuml/labels/simple.py
--rw-r--r--   0        0        0    10593 2023-06-15 15:41:12.568618 pynuml-23.6.0/pynuml/labels/standard.py
--rw-r--r--   0        0        0       28 2023-05-23 17:23:11.335591 pynuml-23.6.0/pynuml/plot/__init__.py
--rw-r--r--   0        0        0     5246 2023-05-23 17:23:11.335785 pynuml-23.6.0/pynuml/plot/graph.py
--rw-r--r--   0        0        0       39 2023-02-27 22:44:16.231786 pynuml-23.6.0/pynuml/process/__init__.py
--rw-r--r--   0        0        0      463 2023-02-27 22:44:16.231898 pynuml-23.6.0/pynuml/process/base.py
--rw-r--r--   0        0        0     6682 2023-06-15 20:05:13.778385 pynuml-23.6.0/pynuml/process/hitgraph.py
--rw-r--r--   0        0        0     3780 2022-10-01 15:34:05.363995 pynuml-23.6.0/pynuml/process/spmap.py
--rw-r--r--   0        0        0      599 2023-06-15 15:15:22.011325 pynuml-23.6.0/pyproject.toml
--rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 pynuml-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2022-08-22 18:47:46.562567 pynuml-23.6.1/.gitignore
+-rw-r--r--   0        0        0      824 2023-06-15 20:05:13.774670 pynuml-23.6.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1074 2023-05-23 17:23:11.333385 pynuml-23.6.1/LICENSE
+-rw-r--r--   0        0        0     5647 2023-05-11 17:09:33.660248 pynuml-23.6.1/README.md
+-rw-r--r--   0        0        0      170 2022-08-22 18:47:46.563031 pynuml-23.6.1/doc/README.md
+-rw-r--r--   0        0        0     9267 2022-08-22 18:47:46.563254 pynuml-23.6.1/doc/graph_create.md
+-rw-r--r--   0        0        0     2903 2022-08-22 18:47:46.563416 pynuml-23.6.1/doc/python_env.md
+-rw-r--r--   0        0        0      638 2023-05-23 17:23:11.333546 pynuml-23.6.1/docs/Makefile
+-rw-r--r--   0        0        0      924 2023-06-26 16:24:16.942644 pynuml-23.6.1/docs/conf.py
+-rw-r--r--   0        0        0      673 2023-06-15 20:05:13.775100 pynuml-23.6.1/docs/index.rst
+-rw-r--r--   0        0        0     1413 2023-06-15 20:05:13.775357 pynuml-23.6.1/docs/install/installation.rst
+-rw-r--r--   0        0        0      804 2023-05-23 17:23:11.333683 pynuml-23.6.1/docs/make.bat
+-rw-r--r--   0        0        0      581 2022-08-22 18:47:46.563608 pynuml-23.6.1/example/plot.py
+-rwxr-xr-x   0        0        0     2089 2022-11-30 18:31:20.903706 pynuml-23.6.1/example/process.py
+-rw-r--r--   0        0        0     1169 2022-08-22 18:47:46.563858 pynuml-23.6.1/h5merge.py
+-rw-r--r--   0        0        0       38 2022-10-01 15:34:05.362452 pynuml-23.6.1/pynuml/.gitignore
+-rw-r--r--   0        0        0      164 2023-06-26 16:24:16.942849 pynuml-23.6.1/pynuml/__init__.py
+-rw-r--r--   0        0        0       97 2023-02-27 22:44:16.230810 pynuml-23.6.1/pynuml/io/__init__.py
+-rw-r--r--   0        0        0    33647 2023-05-23 17:23:11.334552 pynuml-23.6.1/pynuml/io/file.py
+-rw-r--r--   0        0        0     3224 2023-06-26 16:24:16.943048 pynuml-23.6.1/pynuml/io/h5interface.py
+-rw-r--r--   0        0        0     4089 2023-05-23 17:23:11.334967 pynuml-23.6.1/pynuml/io/out.py
+-rw-r--r--   0        0        0      102 2023-06-15 20:05:13.776689 pynuml-23.6.1/pynuml/labels/__init__.py
+-rw-r--r--   0        0        0     1476 2022-10-01 15:34:05.363366 pynuml-23.6.1/pynuml/labels/ccqe.py
+-rw-r--r--   0        0        0     1156 2023-06-15 20:05:13.776860 pynuml-23.6.1/pynuml/labels/flavor.py
+-rw-r--r--   0        0        0      779 2023-05-23 17:23:11.335229 pynuml-23.6.1/pynuml/labels/simple.py
+-rw-r--r--   0        0        0    10593 2023-06-15 15:41:12.568618 pynuml-23.6.1/pynuml/labels/standard.py
+-rw-r--r--   0        0        0       28 2023-05-23 17:23:11.335591 pynuml-23.6.1/pynuml/plot/__init__.py
+-rw-r--r--   0        0        0     5246 2023-05-23 17:23:11.335785 pynuml-23.6.1/pynuml/plot/graph.py
+-rw-r--r--   0        0        0       39 2023-02-27 22:44:16.231786 pynuml-23.6.1/pynuml/process/__init__.py
+-rw-r--r--   0        0        0      463 2023-02-27 22:44:16.231898 pynuml-23.6.1/pynuml/process/base.py
+-rw-r--r--   0        0        0     6703 2023-06-23 18:03:06.407000 pynuml-23.6.1/pynuml/process/hitgraph.py
+-rw-r--r--   0        0        0     3780 2022-10-01 15:34:05.363995 pynuml-23.6.1/pynuml/process/spmap.py
+-rw-r--r--   0        0        0      599 2023-06-15 15:15:22.011325 pynuml-23.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 pynuml-23.6.1/PKG-INFO
```

### Comparing `pynuml-23.6.0/.readthedocs.yaml` & `pynuml-23.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/LICENSE` & `pynuml-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/README.md` & `pynuml-23.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/doc/graph_create.md` & `pynuml-23.6.1/doc/graph_create.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/doc/python_env.md` & `pynuml-23.6.1/doc/python_env.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/docs/Makefile` & `pynuml-23.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/docs/conf.py` & `pynuml-23.6.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'pynuml'
 copyright = '2023, v hewes'
 author = 'v hewes'
-release = '0.1.1'
+release = '23.6.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `pynuml-23.6.0/docs/index.rst` & `pynuml-23.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/docs/install/installation.rst` & `pynuml-23.6.1/docs/install/installation.rst`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/docs/make.bat` & `pynuml-23.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/example/plot.py` & `pynuml-23.6.1/example/plot.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/example/process.py` & `pynuml-23.6.1/example/process.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/h5merge.py` & `pynuml-23.6.1/h5merge.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/io/file.py` & `pynuml-23.6.1/pynuml/io/file.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/io/h5interface.py` & `pynuml-23.6.1/pynuml/io/h5interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,23 +65,21 @@
         ds = self.f.create_dataset(f'/dataset/{name}', shape=(), dtype=ctype, data=self._data)
         del ctype, self._fields, self._data, ds
 
     def load_heterodata(self, name: str) -> HeteroData:
         data = HeteroData()
         # Read the whole dataset idx, dataset name is self.groups[idx]
         group = self.f[f'dataset/{name}'][()]
-        dataset_names = group.dtype.names
-
-        for dataset in dataset_names:
+        for dataset in group.dtype.names:
             store, attr = dataset.split('/')
             if "_" in store: store = tuple(store.split("_"))
-            if attr in ['run','subrun','event','num_nodes']: # scalar
-                data[store][attr] = torch.as_tensor(group[dataset][()])
-            elif group[dataset].ndim == 0:
-                # other zero-dimensional size datasets
-                data[store][attr] = torch.LongTensor([[],[]])
+            if group[dataset].ndim == 0:
+                if attr == 'edge_index': # empty edge tensor
+                    data[store][attr] = torch.LongTensor([[],[]])
+                else: # scalar
+                    data[store][attr] = torch.as_tensor(group[dataset][()])
             else: # multi-dimension array
                 data[store][attr] = torch.as_tensor(group[dataset][:])
         return data
 
     def keys(self) -> list[str]:
         return list(self.f['dataset'].keys())
```

### Comparing `pynuml-23.6.0/pynuml/io/out.py` & `pynuml-23.6.1/pynuml/io/out.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/labels/ccqe.py` & `pynuml-23.6.1/pynuml/labels/ccqe.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/labels/flavor.py` & `pynuml-23.6.1/pynuml/labels/flavor.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/labels/simple.py` & `pynuml-23.6.1/pynuml/labels/simple.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/labels/standard.py` & `pynuml-23.6.1/pynuml/labels/standard.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/plot/graph.py` & `pynuml-23.6.1/pynuml/plot/graph.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pynuml/process/hitgraph.py` & `pynuml-23.6.1/pynuml/process/hitgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,10 +157,10 @@
             data[p, 'nexus', 'sp'].edge_index = edge3d.long()
 
             # truth information
             if self.semantic_labeller:
                 data[p].y_semantic = torch.tensor(plane_hits['semantic_label'].fillna(-1).values).long()
                 data[p].y_instance = torch.tensor(plane_hits['instance_label'].fillna(-1).values).long()
             if self.event_labeller:
-                data['evt'].y = self.event_labeller(evt['event_table'])
+                data['evt'].y = torch.tensor(self.event_labeller(evt['event_table'])).long()
 
         return evt.name, data
```

### Comparing `pynuml-23.6.0/pynuml/process/spmap.py` & `pynuml-23.6.1/pynuml/process/spmap.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/pyproject.toml` & `pynuml-23.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.0/PKG-INFO` & `pynuml-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynuml
-Version: 23.6.0
+Version: 23.6.1
 Summary: Standardised ML input processing for particle physics
 Author-email: v hewes <vhewes@fnal.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: h5py>=3.7.0
```

