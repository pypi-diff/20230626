# Comparing `tmp/moldoc-1.1.0.tar.gz` & `tmp/moldoc-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moldoc-1.1.0.tar", last modified: Tue Jun 20 14:39:00 2023, max compression
+gzip compressed data, was "moldoc-2.0.0.tar", last modified: Mon Jun 26 15:54:42 2023, max compression
```

## Comparing `moldoc-1.1.0.tar` & `moldoc-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.331547 moldoc-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.323547 moldoc-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 14:38:19.000000 moldoc-1.1.0/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 14:38:19.000000 moldoc-1.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 14:38:19.000000 moldoc-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 14:38:19.000000 moldoc-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-20 14:39:00.331547 moldoc-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-20 14:38:19.000000 moldoc-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)   117976 2023-06-20 14:38:19.000000 moldoc-1.1.0/configuration.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 14:38:19.000000 moldoc-1.1.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)  1268442 2023-06-20 14:38:19.000000 moldoc-1.1.0/moldoc.gif
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-20 14:38:19.000000 moldoc-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:39:00.331547 moldoc-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.323547 moldoc-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc/_internal/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/mesh_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/scene_config.py
--rw-r--r--   0 runner    (1001) docker     (123)   351667 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/molDraw.js
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/moldoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)   551410 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/three.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.331547 moldoc-1.1.0/tests/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.331547 moldoc-1.1.0/tests/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/source/_static/empty
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.329191 moldoc-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.313191 moldoc-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.317191 moldoc-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-26 15:54:13.000000 moldoc-2.0.0/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 15:54:13.000000 moldoc-2.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 15:54:13.000000 moldoc-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-26 15:54:13.000000 moldoc-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-26 15:54:42.325191 moldoc-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-26 15:54:13.000000 moldoc-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   117976 2023-06-26 15:54:13.000000 moldoc-2.0.0/configuration.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 15:54:13.000000 moldoc-2.0.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)  1268442 2023-06-26 15:54:13.000000 moldoc-2.0.0/moldoc.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-26 15:54:13.000000 moldoc-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:54:42.329191 moldoc-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.313191 moldoc-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.321191 moldoc-2.0.0/src/moldoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.321191 moldoc-2.0.0/src/moldoc/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.325191 moldoc-2.0.0/src/moldoc/_internal/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/mesh_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/javascript/scene_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   351667 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/molDraw.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/moldoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551410 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/_internal/three.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:13.000000 moldoc-2.0.0/src/moldoc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 15:54:42.000000 moldoc-2.0.0/src/moldoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.321191 moldoc-2.0.0/src/moldoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-26 15:54:42.000000 moldoc-2.0.0/src/moldoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 15:54:42.000000 moldoc-2.0.0/src/moldoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:54:42.000000 moldoc-2.0.0/src/moldoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 15:54:42.000000 moldoc-2.0.0/src/moldoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:54:42.000000 moldoc-2.0.0/src/moldoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.325191 moldoc-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 15:54:13.000000 moldoc-2.0.0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-26 15:54:13.000000 moldoc-2.0.0/tests/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.325191 moldoc-2.0.0/tests/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:42.325191 moldoc-2.0.0/tests/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:13.000000 moldoc-2.0.0/tests/source/_static/empty
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-26 15:54:13.000000 moldoc-2.0.0/tests/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-26 15:54:13.000000 moldoc-2.0.0/tests/source/index.rst
```

### Comparing `moldoc-1.1.0/.github/workflows/publish_release.yaml` & `moldoc-2.0.0/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/.github/workflows/tests.yaml` & `moldoc-2.0.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/LICENSE` & `moldoc-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/PKG-INFO` & `moldoc-2.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: moldoc
-Version: 1.1.0
-Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
-Project-URL: github, https://github.com/lukasturcani/moldoc
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 :author: Lukas Turcani
 
 Introduction
 ============
 
 ``moldoc`` is a Sphinx extension for making better chemistry
 documentation. It allows you to embed 3D, interactive models of
@@ -146,14 +136,30 @@
 
         print('In some_fn()')
 
 
 Configuration
 =============
 
+Global
+------
+
+You can use the ``moldoc_default_molecule_config`` to set the default
+``MoleculeConfig`` value for all renderings. This is defined in ``conf.py``:
+
+.. code-block:: python
+
+  import moldoc.molecule as molecule
+  moldoc_default_molecule_config = molecule.MoleculeConfig(
+      background_color=molecule.Color(32, 32, 32),
+  )
+
+Local
+-----
+
 The display of molecules is pretty configurable, here is a snapshot of
 the different configuration options you have, but note that this is
 not an exhaustive list
 
 .. image:: configuration.jpg
 
 Configuration happens on both the molecule and the atom level. For
```

### Comparing `moldoc-1.1.0/README.rst` & `moldoc-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: moldoc
+Version: 2.0.0
+Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
+Project-URL: github, https://github.com/lukasturcani/moldoc
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 :author: Lukas Turcani
 
 Introduction
 ============
 
 ``moldoc`` is a Sphinx extension for making better chemistry
 documentation. It allows you to embed 3D, interactive models of
@@ -136,14 +146,30 @@
 
         print('In some_fn()')
 
 
 Configuration
 =============
 
+Global
+------
+
+You can use the ``moldoc_default_molecule_config`` to set the default
+``MoleculeConfig`` value for all renderings. This is defined in ``conf.py``:
+
+.. code-block:: python
+
+  import moldoc.molecule as molecule
+  moldoc_default_molecule_config = molecule.MoleculeConfig(
+      background_color=molecule.Color(32, 32, 32),
+  )
+
+Local
+-----
+
 The display of molecules is pretty configurable, here is a snapshot of
 the different configuration options you have, but note that this is
 not an exhaustive list
 
 .. image:: configuration.jpg
 
 Configuration happens on both the molecule and the atom level. For
```

### Comparing `moldoc-1.1.0/configuration.jpg` & `moldoc-2.0.0/configuration.jpg`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/moldoc.gif` & `moldoc-2.0.0/moldoc.gif`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/pyproject.toml` & `moldoc-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/javascript/atoms.py` & `moldoc-2.0.0/src/moldoc/_internal/javascript/atoms.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/javascript/material.py` & `moldoc-2.0.0/src/moldoc/_internal/javascript/material.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/javascript/mesh_config.py` & `moldoc-2.0.0/src/moldoc/_internal/javascript/mesh_config.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/javascript/scene_config.py` & `moldoc-2.0.0/src/moldoc/_internal/javascript/scene_config.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/molDraw.js` & `moldoc-2.0.0/src/moldoc/_internal/molDraw.js`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/moldoc.py` & `moldoc-2.0.0/src/moldoc/_internal/moldoc.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,18 @@
     else:
         molecule_config = default_molecule_config
 
     moldoc_node_id = node.get_moldoc_name()
 
     if not getattr(self, "moldoc_scripts_added", False):
         self.body.append(
-            '<script src="/_static/three.min.js"></script>'
-            '<script src="/_static/molDraw.js"></script>'
+            '<script src="three.min.js"></script>'
+            '<script src="molDraw.js"></script>'
+            '<script src="../three.min.js"></script>'
+            '<script src="../molDraw.js"></script>'
             "<script>const md=molDraw;"
             "let atoms=[];"
             "let bonds=[];"
             "let maybeMolecule=undefined;"
             "</script>"
         )
         self.moldoc_scripts_added = True
```

### Comparing `moldoc-1.1.0/src/moldoc/_internal/molecule.py` & `moldoc-2.0.0/src/moldoc/_internal/molecule.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/_internal/three.min.js` & `moldoc-2.0.0/src/moldoc/_internal/three.min.js`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc/molecule.py` & `moldoc-2.0.0/src/moldoc/molecule.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/src/moldoc.egg-info/PKG-INFO` & `moldoc-2.0.0/src/moldoc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moldoc
-Version: 1.1.0
+Version: 2.0.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/moldoc
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -146,14 +146,30 @@
 
         print('In some_fn()')
 
 
 Configuration
 =============
 
+Global
+------
+
+You can use the ``moldoc_default_molecule_config`` to set the default
+``MoleculeConfig`` value for all renderings. This is defined in ``conf.py``:
+
+.. code-block:: python
+
+  import moldoc.molecule as molecule
+  moldoc_default_molecule_config = molecule.MoleculeConfig(
+      background_color=molecule.Color(32, 32, 32),
+  )
+
+Local
+-----
+
 The display of molecules is pretty configurable, here is a snapshot of
 the different configuration options you have, but note that this is
 not an exhaustive list
 
 .. image:: configuration.jpg
 
 Configuration happens on both the molecule and the atom level. For
```

### Comparing `moldoc-1.1.0/src/moldoc.egg-info/SOURCES.txt` & `moldoc-2.0.0/src/moldoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/tests/Makefile` & `moldoc-2.0.0/tests/Makefile`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/tests/make.bat` & `moldoc-2.0.0/tests/make.bat`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/tests/source/conf.py` & `moldoc-2.0.0/tests/source/conf.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.1.0/tests/source/index.rst` & `moldoc-2.0.0/tests/source/index.rst`

 * *Files identical despite different names*

