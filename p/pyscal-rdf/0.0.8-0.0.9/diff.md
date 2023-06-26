# Comparing `tmp/pyscal_rdf-0.0.8.tar.gz` & `tmp/pyscal_rdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.0.8.tar", last modified: Mon Jun 26 14:44:03 2023, max compression
+gzip compressed data, was "pyscal_rdf-0.0.9.tar", last modified: Mon Jun 26 19:43:48 2023, max compression
```

## Comparing `pyscal_rdf-0.0.8.tar` & `pyscal_rdf-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/pyscal_rdf/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/rdfsystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/pyscal_rdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 14:44:03.000000 pyscal_rdf-0.0.8/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 14:44:02.000000 pyscal_rdf-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:44:03.212879 pyscal_rdf-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-26 14:43:57.000000 pyscal_rdf-0.0.8/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:43:48.497142 pyscal_rdf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 19:43:48.497142 pyscal_rdf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:43:48.497142 pyscal_rdf-0.0.9/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36897 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/rdfsystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/pyscal_rdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:43:48.497142 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:43:48.497142 pyscal_rdf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 19:43:48.000000 pyscal_rdf-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:43:48.497142 pyscal_rdf-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-26 19:43:44.000000 pyscal_rdf-0.0.9/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.0.8/LICENSE` & `pyscal_rdf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/PKG-INFO` & `pyscal_rdf-0.0.9/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyscal_rdf
-Version: 0.0.8
+Name: pyscal-rdf
+Version: 0.0.9
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.0.8/README.md` & `pyscal_rdf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/graph.py` & `pyscal_rdf-0.0.9/pyscal_rdf/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,21 +672,30 @@
 
 
     def inspect_sample(self, sample=None):
         if sample is None:
             sample = self.sample
         natoms = self.graph.value(sample, CMSO.hasNumberOfAtoms).toPython()
         material = list([k[2] for k in self.graph.triples((sample, CMSO.hasMaterial, None))])[0]
-        defects = list([k[2] for k in self.graph.triples((material, CMSO.hasDefect, None))]) 
+        defects = list([k[2] for k in self.graph.triples((material, CMSO.hasDefect, None))])
+        composition = list([k[2].toPython() for k in self.graph.triples((material, CMSO.hasElementRatio, None))])
+        crystalstructure = self.graph.value(material, CMSO.hasStructure)
+        spacegroupsymbol = self.graph.value(crystalstructure, CMSO.hasSpaceGroupSymbol).toPython()
+
+        lattice = self.graph.value(sample, CMSO.hasNumberOfAtoms).toPython()
         defect_types = list([self.graph.value(d, RDF.type).toPython() for d in defects])
         props = list([k[2].toPython() for k in self.graph.triples((sample, CMSO.hasCalculatedProperty, None))])
         propvals = list([self.graph.value(d, CMSO.hasValue).toPython() for d in props])
         units = list([self.graph.value(d, CMSO.hasUnit).toPython() for d in props])
         st = []
         st.append(f'Sample with {natoms} atoms.\n')
+        st.append("Material:\n")
+        st.append(" ".join(composition))
+        st.append("\n")
+        st.append(f'Space Group symbol: {spacegroupsymbol}\n')
         if len(defect_types) > 0:
             st.append('With defects:\n')
             for d in defect_types:
                 st.append(f'{d}\n')
         if len(props) > 0:
             st.append('With calculated properties:\n')
             for x in range(len(props)):
```

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/json_io.py` & `pyscal_rdf-0.0.9/pyscal_rdf/json_io.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/network.py` & `pyscal_rdf-0.0.9/pyscal_rdf/network.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/properties.py` & `pyscal_rdf-0.0.9/pyscal_rdf/properties.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/queries.py` & `pyscal_rdf-0.0.9/pyscal_rdf/queries.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/rdfsystem.py` & `pyscal_rdf-0.0.9/pyscal_rdf/rdfsystem.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/structure.py` & `pyscal_rdf-0.0.9/pyscal_rdf/structure.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf/visualize.py` & `pyscal_rdf-0.0.9/pyscal_rdf/visualize.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyscal-rdf
-Version: 0.0.8
+Name: pyscal_rdf
+Version: 0.0.9
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.0.8/pyscal_rdf.egg-info/SOURCES.txt` & `pyscal_rdf-0.0.9/pyscal_rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/setup.py` & `pyscal_rdf-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal_rdf',
-    version='0.0.8',
+    version='0.0.9',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['pyscal_rdf', 'pyscal_rdf.*']),
     zip_safe=False,
```

### Comparing `pyscal_rdf-0.0.8/tests/test_encoder_and_write.py` & `pyscal_rdf-0.0.9/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/tests/test_graph.py` & `pyscal_rdf-0.0.9/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/tests/test_queries.py` & `pyscal_rdf-0.0.9/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.8/tests/test_structuregraph.py` & `pyscal_rdf-0.0.9/tests/test_structuregraph.py`

 * *Files identical despite different names*

