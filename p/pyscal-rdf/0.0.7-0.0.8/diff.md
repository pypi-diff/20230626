# Comparing `tmp/pyscal_rdf-0.0.7.tar.gz` & `tmp/pyscal_rdf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.0.7.tar", last modified: Fri Jun 23 10:59:43 2023, max compression
+gzip compressed data, was "pyscal_rdf-0.0.8.tar", last modified: Mon Jun 26 14:44:03 2023, max compression
```

## Comparing `pyscal_rdf-0.0.7.tar` & `pyscal_rdf-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.856590 pyscal_rdf-0.0.7/pyscal_rdf/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    33695 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.856590 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/rdfsystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 14:44:02.000000 pyscal_rdf-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.0.7/LICENSE` & `pyscal_rdf-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/PKG-INFO` & `pyscal_rdf-0.0.8/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyscal_rdf
-Version: 0.0.7
+Name: pyscal-rdf
+Version: 0.0.8
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -24,15 +24,27 @@
 
 ## Installation
 
 ### Supported operating systems
 
 `pyscal_rdf` can be installed on Linux and Mac OS based systems. On Windows systems, it is recommended to use  [Windows subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install).
 
-### Using a conda environment
+### Using pip
+
+```
+pip install pyscal-rdf
+```
+### Using conda
+
+```
+conda install -c conda-forge pyscal-rdf
+```
+
+
+### Building from the repository
 
 We strongly recommend creating a conda environment for the installation. To see how you can install conda see [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/).
 
 Once a conda distribution is available, the following steps will help set up an environment to use `pyscal_rdf`. First step is to clone the repository.
 
 ```
 git clone https://github.com/pyscal/pyscal_rdf.git
```

### Comparing `pyscal_rdf-0.0.7/README.md` & `pyscal_rdf-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,27 @@
 
 ## Installation
 
 ### Supported operating systems
 
 `pyscal_rdf` can be installed on Linux and Mac OS based systems. On Windows systems, it is recommended to use  [Windows subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install).
 
-### Using a conda environment
+### Using pip
+
+```
+pip install pyscal-rdf
+```
+### Using conda
+
+```
+conda install -c conda-forge pyscal-rdf
+```
+
+
+### Building from the repository
 
 We strongly recommend creating a conda environment for the installation. To see how you can install conda see [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/).
 
 Once a conda distribution is available, the following steps will help set up an environment to use `pyscal_rdf`. First step is to clone the repository.
 
 ```
 git clone https://github.com/pyscal/pyscal_rdf.git
```

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/graph.py` & `pyscal_rdf-0.0.8/pyscal_rdf/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 """
 
 from rdflib import Graph, Literal, Namespace, XSD, RDF, RDFS, BNode, URIRef, FOAF, SKOS, DCTERMS
 from rdflib.store import NO_STORE, VALID_STORE
 
 import os
 import numpy as np
+import inspect
 from ase.io import write
+import copy
 
 from pyscal_rdf.visualize import visualize_graph
 from pyscal_rdf.network import OntologyNetwork
+from pyscal_rdf.rdfsystem import System
 import pyscal_rdf.properties as prp
-from pyscal3.core import System
+#from pyscal3.core import System
 from pyscal3.atoms import Atoms
-from pyscal3.core import System
 
 CMSO = Namespace("https://purls.helmholtz-metadaten.de/cmso/")
 PLDO = Namespace("https://purls.helmholtz-metadaten.de/pldo/")
 PODO = Namespace("https://purls.helmholtz-metadaten.de/podo/")
 
 defstyledict = {
     "BNode": {"color": "#ffe6ff", 
@@ -48,35 +50,54 @@
     return refdict
 
 class RDFGraph:
     def __init__(self, graph_file=None, 
         store="Memory", 
         store_file=None,
         identifier="default_graph"):
-        self.graph = Graph(store=store, identifier=identifier)
+        
         #owlfile = os.path.join(os.path.dirname(__file__), "data/cmso.owl")
         #self.graph.parse(owlfile, format='xml')
-        if store != "Memory":
-            if not store=="SQLAlchemy":
-                raise ValueError("Only SQLAlchemy store is supported")
+        if store == "Memory":
+            self.graph = Graph(store="Memory", identifier=identifier)
+
+        elif store=="SQLAlchemy":
             if store_file is None:
                 raise ValueError("store file is needed if store is not memory")
+            self.graph = Graph(store="SQLAlchemy", identifier=identifier)
             uri = Literal(f"sqlite:///{store_file}")
             self.graph.open(uri, create=True)
+
+        elif inspect.isclass(type(store)):
+            try:
+                prpath = store.path
+                dbfile = os.path.join(prpath, 'project.db')
+                #now start sqlalchemy instance
+                self.graph = Graph(store="SQLAlchemy", identifier=identifier)
+                uri = Literal(f"sqlite:///{dbfile}")
+                self.graph.open(uri, create=True)
+            except:
+                raise ValueError("store should be pyiron_project, SQLAlchemy, or Memory")
+        
+        else:
+            raise ValueError("store should be pyiron_project, SQLAlchemy, or Memory")
+
         self.graph.bind("cmso", CMSO)
         self.graph.bind("pldo", PLDO)
         
         if graph_file is not None:
             if os.path.exists(graph_file):
                 self.graph.parse(graph_file)
+        
         self.sample = None
         self.material = None
         self.sysdict = None
         self.sgraph = None
         self._query_graph = OntologyNetwork()
+        self._atom_ids = None
     
     def process_structure(self, structure, format=None):
         """
         Convert a given :py:class:`pyscal.core.System` to a data dictionary which can be used for annotation
         and storing the data in the RDF Graph.
 
         Parameters
@@ -185,15 +206,15 @@
         #        return self.sysdict[key]
         return None
     
     def add(self, triple):
         if str(triple[2].toPython()) != 'None':
             self.graph.add(triple)
         
-    def add_structure_to_graph(self, structure, names=False, name_index=None, format=None):
+    def add_structure_to_graph(self, structure, names=True, name_index=None, format=None):
         """
         Add a given :py:class:`pyscal.core.System` to the Graph object
 
         Parameters
         ----------
         structure: :py:class:`pyscal.core.System`
             input structure
@@ -206,15 +227,17 @@
         None
         """
         self.process_structure(structure, format=format)
         #now add to graph
         if name_index is None:
             name_index = self.n_samples + 1
         self.create_graph(names=names, name_index=name_index)
-        
+        structure.sample = self.sample
+        structure._atom_ids = copy.copy(self._atom_ids)
+        structure.graph = self
     
     def create_graph(self, names=False, name_index="1"):
         """
         Create the RDF Graph from the data stored
 
         Parameters
         ----------
@@ -505,21 +528,23 @@
         ----------
         name
             if provided, the name will be used instead of random identifier
 
         Returns
         -------
         """
+        self._atom_ids = []
 
         for x in range(len(self.data("Positions"))):
             uname = None
             if name is not None:
                 uname = f'{name}_{x}'            
             #create atom
             atom = BNode(uname)
+            self._atom_ids.append(atom)
             self.add((self.sample, CMSO.hasAtom, atom))
             self.add((atom, RDF.type, CMSO.Atom))
 
             uname = None
             if name is not None:
                 uname = f'{name}_{x}_Position'            
             position = BNode(uname)
@@ -627,14 +652,51 @@
 
         vacancy_01 = BNode(name)
         self.add((self.material, CMSO.hasDefect, vacancy_01))
         self.add((vacancy_01, RDF.type, PODO.Vacancy))
         self.add((self.simulation_cell, PODO.hasVacancyConcentration, Literal(concentration, datatype=XSD.float)))
         if number is not None:
             self.add((self.simulation_cell, PODO.hasNumberOfVacancies, Literal(number, datatype=XSD.integer)))
+        #if vacancy is added, atoms have to be deleted from the existing record!
+        #this is indeed a tricky item
+
+
+    def add_calculated_quantity(self, propertyname, value, unit=None, sample=None):
+        prop = BNode(propertyname)
+        if sample is None:
+            sample = self.sample
+        self.add((sample, CMSO.hasCalculatedProperty, prop))
+        self.add((prop, RDF.type, CMSO.CalculatedProperty))
+        self.add((prop, CMSO.hasValue, Literal(value)))
+        if unit is not None:
+            self.add((prop, CMSO.hasUnit, URIRef(f'https://qudt.org/2.1/vocab/unit#{unit}')))
+
+
+    def inspect_sample(self, sample=None):
+        if sample is None:
+            sample = self.sample
+        natoms = self.graph.value(sample, CMSO.hasNumberOfAtoms).toPython()
+        material = list([k[2] for k in self.graph.triples((sample, CMSO.hasMaterial, None))])[0]
+        defects = list([k[2] for k in self.graph.triples((material, CMSO.hasDefect, None))]) 
+        defect_types = list([self.graph.value(d, RDF.type).toPython() for d in defects])
+        props = list([k[2].toPython() for k in self.graph.triples((sample, CMSO.hasCalculatedProperty, None))])
+        propvals = list([self.graph.value(d, CMSO.hasValue).toPython() for d in props])
+        units = list([self.graph.value(d, CMSO.hasUnit).toPython() for d in props])
+        st = []
+        st.append(f'Sample with {natoms} atoms.\n')
+        if len(defect_types) > 0:
+            st.append('With defects:\n')
+            for d in defect_types:
+                st.append(f'{d}\n')
+        if len(props) > 0:
+            st.append('With calculated properties:\n')
+            for x in range(len(props)):
+                st.append(f'{props[x]} with value: {propvals[x]} and unit: {units[x]}\n')
+
+        return " ".join(st)
 
     def visualize(self, *args, **kwargs):
         """
         Vosualise the RDF tree of the Graph
 
         Parameters
         ----------
```

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/json_io.py` & `pyscal_rdf-0.0.8/pyscal_rdf/json_io.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/network.py` & `pyscal_rdf-0.0.8/pyscal_rdf/network.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/properties.py` & `pyscal_rdf-0.0.8/pyscal_rdf/properties.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/queries.py` & `pyscal_rdf-0.0.8/pyscal_rdf/queries.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/structure.py` & `pyscal_rdf-0.0.8/pyscal_rdf/structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 StructureGraph is the central object in pyscal_rdf which combines all the functionality
 of :py:class:`pyscal_rdf.graph.RDFGraph` along with easy structural creation routines.
 """
 import numpy as np
-from pyscal3.core import System
+import copy
+
+from pyscal_rdf.rdfsystem import System
 from pyscal3.crystal_structures import structure_creator, elements, structures
 from pyscal_rdf.graph import RDFGraph
 from pyscal3.grain_boundary import GrainBoundary
 
 class StructureGraph(RDFGraph):
     def __init__(self, graph_file=None, 
         store="Memory", 
         store_file=None,
         identifier="default_graph"):
+        
         super().__init__(graph_file=graph_file, store=store, store_file=store_file, identifier=identifier)
         self._element_dict = elements
         self._structure_dict = structures
-        
+
     def create_element(self, element, repetitions=(1,1,1), 
-                       noise=0, add_to_graph=True, names=False):
+                       noise=0, add_to_graph=True, names=True):
         """
         Create a crystal structure of the given element
 
         Parameters
         ----------
         element : string
             chemical symbol of the element
@@ -48,28 +51,31 @@
         -----
         Python module Mendelev is used to get the lattice constant with which the system will be constructed.
         If it is an hexagonal lattice, the ideal c/a ration will be used.
 
         """
         if element in self._element_dict.keys():
             structure = self._element_dict[element]['structure']
-            sys = structure_creator(structure,
+            sys = System(source=structure_creator(structure,
                         repetitions=repetitions,
                         noise=noise,
                         lattice_constant=self._element_dict[element]['lattice_constant'],
-                        element = element)
+                        element = element))
             if add_to_graph:
                 self.add_structure_to_graph(sys, names=names)
+                #sys.sample = self.sample
+                #sys._atom_ids = copy.copy(self._atom_ids)
+                #sys.graph = self
             return sys
     
     def create_structure(self, structure, 
                          lattice_constant = 1.00, 
                          repetitions = None, ca_ratio = 1.633, 
                          noise = 0, element=None,
-                         add_to_graph=True, names=False):
+                         add_to_graph=True, names=True):
         """
         Create a crystal structure and return it as a System object.
 
         Parameters
         ----------
         structure : {'sc', 'bcc', 'fcc', 'hcp', 'diamond', 'a15' or 'l12'}
             type of the crystal structure
@@ -98,26 +104,29 @@
 
         Returns
         -------
         System: pyscal System
 
         """
         if structure in self._structure_dict.keys():
-            sys = structure_creator(structure,
+            sys = System(source=structure_creator(structure,
                         repetitions=repetitions,
                         noise=noise,
                         lattice_constant=lattice_constant,
                         element = element,
-                        )
+                        ))
             if add_to_graph:
                 self.add_structure_to_graph(sys, names = names)
+                #sys.sample = self.sample
+                #sys._atom_ids = copy.copy(self._atom_ids)
+                #sys.graph = self
             return sys
     
     def read_structure(self, filename, format="lammps-dump",
-                      add_to_graph=True, names=False):
+                      add_to_graph=True, names=True):
         """
         Read an input file and return it as a System object.
 
         Parameters
         ----------
         filename: string
             name of the input file
@@ -136,25 +145,28 @@
         System: pyscal System
         system will be populated with given atoms and simulation box
 
         """
         sys = System(filename, format=format)
         if add_to_graph:
             self.add_structure_to_graph(sys, names=names)
+            #sys.sample = self.sample
+            #sys._atom_ids = copy.copy(self._atom_ids)
+            #sys.graph = self
         return sys
     
     def create_grain_boundary(self, axis, 
                               sigma, gb_plane,
                               structure=None,
                               element=None, 
                               lattice_constant=1,
                               repetitions=(1,1,1),
                               overlap=0.0,
                               add_to_graph=True,
-                              names=False):
+                              names=True):
         """
         Create a grain boundary structure and return it as a System object.
 
         Parameters
         ----------
         axis: list of ints of length 3
             The grain boundary axis
@@ -194,27 +206,30 @@
         """
         gb = GrainBoundary()
         gb.create_grain_boundary(axis=axis, sigma=sigma, 
                                  gb_plane=gb_plane)
 
         #use standard creation routine
         if structure is not None:
-            sys = gb.populate_grain_boundary(structure, 
+            sys = System(source=gb.populate_grain_boundary(structure, 
                                              repetitions = repetitions,
                                              lattice_parameter = lattice_constant,
-                                             overlap=overlap)
+                                             overlap=overlap))
         elif element is not None:
-            sys = gb.populate_grain_boundary(element, 
+            sys = System(source=gb.populate_grain_boundary(element, 
                                              repetitions=repetitions,
-                                             overlap=overlap)
+                                             overlap=overlap))
         else:
             raise ValueError("Either structure or element should be provided")
             
         #mapping of the system can be done
         self.add_structure_to_graph(sys, names=names)
+        #sys.sample = self.sample
+        #sys._atom_ids = copy.copy(self._atom_ids)
+        #sys.graph = self
         gb_dict = {"GBPlane": " ".join(np.array(gb_plane).astype(str)),
                   "RotationAxis": axis,
                   "MisorientationAngle": gb.theta,
                   "GBType": gb.find_gb_character(),
                   "sigma": gb.sigma,
                   }
         self.add_gb(gb_dict)
```

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf/visualize.py` & `pyscal_rdf-0.0.8/pyscal_rdf/visualize.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyscal-rdf
-Version: 0.0.7
+Name: pyscal_rdf
+Version: 0.0.8
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -24,15 +24,27 @@
 
 ## Installation
 
 ### Supported operating systems
 
 `pyscal_rdf` can be installed on Linux and Mac OS based systems. On Windows systems, it is recommended to use  [Windows subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install).
 
-### Using a conda environment
+### Using pip
+
+```
+pip install pyscal-rdf
+```
+### Using conda
+
+```
+conda install -c conda-forge pyscal-rdf
+```
+
+
+### Building from the repository
 
 We strongly recommend creating a conda environment for the installation. To see how you can install conda see [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/).
 
 Once a conda distribution is available, the following steps will help set up an environment to use `pyscal_rdf`. First step is to clone the repository.
 
 ```
 git clone https://github.com/pyscal/pyscal_rdf.git
```

### Comparing `pyscal_rdf-0.0.7/pyscal_rdf.egg-info/SOURCES.txt` & `pyscal_rdf-0.0.8/pyscal_rdf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyscal_rdf/__init__.py
 pyscal_rdf/encoder.py
 pyscal_rdf/graph.py
 pyscal_rdf/json_io.py
 pyscal_rdf/network.py
 pyscal_rdf/properties.py
 pyscal_rdf/queries.py
+pyscal_rdf/rdfsystem.py
 pyscal_rdf/structure.py
 pyscal_rdf/visualize.py
 pyscal_rdf.egg-info/PKG-INFO
 pyscal_rdf.egg-info/SOURCES.txt
 pyscal_rdf.egg-info/dependency_links.txt
 pyscal_rdf.egg-info/not-zip-safe
 pyscal_rdf.egg-info/requires.txt
```

### Comparing `pyscal_rdf-0.0.7/setup.py` & `pyscal_rdf-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal_rdf',
-    version='0.0.7',
+    version='0.0.8',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['pyscal_rdf', 'pyscal_rdf.*']),
     zip_safe=False,
```

### Comparing `pyscal_rdf-0.0.7/tests/test_encoder_and_write.py` & `pyscal_rdf-0.0.8/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/tests/test_graph.py` & `pyscal_rdf-0.0.8/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/tests/test_queries.py` & `pyscal_rdf-0.0.8/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.7/tests/test_structuregraph.py` & `pyscal_rdf-0.0.8/tests/test_structuregraph.py`

 * *Files identical despite different names*

