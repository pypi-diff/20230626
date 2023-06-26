# Comparing `tmp/meow-sim-0.6.8.tar.gz` & `tmp/meow-sim-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.8.tar", last modified: Fri Jun 23 19:54:30 2023, max compression
+gzip compressed data, was "meow-sim-0.6.9.tar", last modified: Mon Jun 26 16:36:12 2023, max compression
```

## Comparing `meow-sim-0.6.8.tar` & `meow-sim-0.6.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-23 19:54:26.000000 meow-sim-0.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-23 19:54:30.403039 meow-sim-0.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-23 19:54:26.000000 meow-sim-0.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     8412 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     3298 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6063 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     4924 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/propagate.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10442 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-23 19:54:26.000000 meow-sim-0.6.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:54:30.403039 meow-sim-0.6.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/tests/
--rw-r--r--   0 root         (0) root         (0)     4135 2023-06-23 19:54:26.000000 meow-sim-0.6.8/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-06-23 19:54:26.000000 meow-sim-0.6.8/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-23 19:54:26.000000 meow-sim-0.6.8/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-26 16:36:07.000000 meow-sim-0.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-26 16:36:12.082835 meow-sim-0.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-26 16:36:07.000000 meow-sim-0.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.078835 meow-sim-0.6.9/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.078835 meow-sim-0.6.9/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.078835 meow-sim-0.6.9/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/propagate.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10442 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-06-26 16:36:07.000000 meow-sim-0.6.9/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 16:36:12.000000 meow-sim-0.6.9/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-26 16:36:07.000000 meow-sim-0.6.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 16:36:12.082835 meow-sim-0.6.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:12.082835 meow-sim-0.6.9/tests/
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-06-26 16:36:07.000000 meow-sim-0.6.9/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-06-26 16:36:07.000000 meow-sim-0.6.9/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-26 16:36:07.000000 meow-sim-0.6.9/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.8/LICENSE` & `meow-sim-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/PKG-INFO` & `meow-sim-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.8
+Version: 0.6.9
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.8/README.md` & `meow-sim-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/__init__.py` & `meow-sim-0.6.9/meow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.8/meow/assets/silicon.csv` & `meow-sim-0.6.9/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.9/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/base_model.py` & `meow-sim-0.6.9/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/cache.py` & `meow-sim-0.6.9/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/cell.py` & `meow-sim-0.6.9/meow/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,42 +57,15 @@
             self.structures, self.materials
         )
         for structures in structures_dict.values():
             _m_full = _create_material_array(self, structures, self.ez_interfaces)
             mask = _m_full > 0
             m_full[mask] = _m_full[mask]
 
-        if self.ez_interfaces:  # fill in 1-pixel gaps
-            mat_x = np.maximum(
-                np.roll(m_full, shift=1, axis=0),
-                np.roll(m_full, shift=-1, axis=0),
-            )
-            mat_y = np.maximum(
-                np.roll(m_full, shift=1, axis=1),
-                np.roll(m_full, shift=-1, axis=1),
-            )
-            mat = mat_x | mat_y
-
-            mask = m_full > 0
-            mask_x = (
-                np.roll(mask, shift=1, axis=0)
-                & (~mask)
-                & np.roll(mask, shift=-1, axis=0)
-            )
-            mask_y = (
-                np.roll(mask, shift=1, axis=1)
-                & (~mask)
-                & np.roll(mask, shift=-1, axis=1)
-            )
-            mask = mask_x | mask_y
-            mask[:1, :] = False
-            mask[-1:, :] = False
-            mask[:, :1] = False
-            mask[:, -1:] = False
-            m_full[mask] = mat[mask]
+        m_full = _fill_single_pixel_gaps(m_full)
 
         return m_full.view(_array)
 
     def _visualize(self, ax=None, cbar=True, show=True):
         import matplotlib.pyplot as plt  # fmt: skip
         from matplotlib.colors import ListedColormap, to_rgba  # fmt: skip
         from mpl_toolkits.axes_grid1 import make_axes_locatable  # fmt: skip
@@ -132,14 +105,15 @@
 
 
 def create_cells(
     structures: List[Structure],
     mesh: Union[Mesh2d, List[Mesh2d]],
     Ls: np.ndarray[Tuple[int], np.dtype[np.float_]],
     z_min: float = 0.0,
+    ez_interfaces: bool = False,
 ) -> List[Cell]:
     """easily create multiple `Cell` objects given a `Mesh` and a collection of cell lengths"""
 
     Ls = np.asarray(Ls, float)
     if Ls.ndim != 1:
         raise ValueError(f"Ls should be 1D. Got shape: {Ls.shape}.")
     if Ls.shape[0] < 0:
@@ -149,15 +123,21 @@
     if len(Ls) != len(meshes):
         raise ValueError(
             f"Number of meshes should correspond to number of lengths (length of Ls). Got {len(meshes)} != {len(Ls)}."
         )
 
     z = np.cumsum(np.concatenate([np.asarray([z_min], float), Ls]))
     cells = [
-        Cell(structures=structures, mesh=mesh, z_min=z_min, z_max=z_max)
+        Cell(
+            structures=structures,
+            mesh=mesh,
+            z_min=z_min,
+            z_max=z_max,
+            ez_interfaces=ez_interfaces,
+        )
         for mesh, (z_min, z_max) in zip(meshes, zip(z[:-1], z[1:]))
     ]
 
     return cells
 
 
 def _create_material_array(cell, structures, ez_interfaces):
@@ -234,7 +214,30 @@
     # don't mask edge of simulation area:
     mask[:, 0] = mask[:, -1] = False
     return mask
 
 
 def _get_boundary_mask_vertical(m_full, negate=False):
     return _get_boundary_mask_horizontal(m_full.T, negate=negate).T
+
+
+def _fill_single_pixel_gaps(m_full):
+    mat_x = np.maximum(
+        np.roll(m_full, shift=1, axis=0),
+        np.roll(m_full, shift=-1, axis=0),
+    )
+    mat_y = np.maximum(
+        np.roll(m_full, shift=1, axis=1),
+        np.roll(m_full, shift=-1, axis=1),
+    )
+    mat = mat_x | mat_y
+
+    mask = m_full > 0
+    mask_x = np.roll(mask, shift=1, axis=0) & (~mask) & np.roll(mask, shift=-1, axis=0)
+    mask_y = np.roll(mask, shift=1, axis=1) & (~mask) & np.roll(mask, shift=-1, axis=1)
+    mask = mask_x | mask_y
+    mask[:1, :] = False
+    mask[-1:, :] = False
+    mask[:, :1] = False
+    mask[:, -1:] = False
+    m_full[mask] = mat[mask]
+    return m_full
```

### Comparing `meow-sim-0.6.8/meow/cross_section.py` & `meow-sim-0.6.9/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/eme/__init__.py` & `meow-sim-0.6.9/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/eme/common.py` & `meow-sim-0.6.9/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/eme/propagate.py` & `meow-sim-0.6.9/meow/eme/propagate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/eme/sax.py` & `meow-sim-0.6.9/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/environment.py` & `meow-sim-0.6.9/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/fde/lumerical.py` & `meow-sim-0.6.9/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/fde/tidy3d.py` & `meow-sim-0.6.9/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/gds_structures.py` & `meow-sim-0.6.9/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/geometries.py` & `meow-sim-0.6.9/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/integrate.py` & `meow-sim-0.6.9/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/materials.py` & `meow-sim-0.6.9/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/mesh.py` & `meow-sim-0.6.9/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/mode.py` & `meow-sim-0.6.9/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/structures.py` & `meow-sim-0.6.9/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow/visualize.py` & `meow-sim-0.6.9/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.9/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.8
+Version: 0.6.9
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.8/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.9/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/pyproject.toml` & `meow-sim-0.6.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.8"
+version = "0.6.9"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.8/tests/test_deserialization.py` & `meow-sim-0.6.9/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/tests/test_mode_operators.py` & `meow-sim-0.6.9/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.8/tests/test_nbs.py` & `meow-sim-0.6.9/tests/test_nbs.py`

 * *Files identical despite different names*

