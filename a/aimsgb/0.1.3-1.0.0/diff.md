# Comparing `tmp/aimsgb-0.1.3.tar.gz` & `tmp/aimsgb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsgb-0.1.3.tar", last modified: Tue May 23 21:21:36 2023, max compression
+gzip compressed data, was "aimsgb-1.0.0.tar", last modified: Mon Jun 26 04:05:56 2023, max compression
```

## Comparing `aimsgb-0.1.3.tar` & `aimsgb-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,44 @@
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-23 21:21:36.320016 aimsgb-0.1.3/
--rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-0.1.3/LICENSE.txt
--rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-23 21:21:36.320140 aimsgb-0.1.3/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-0.1.3/README.rst
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-23 21:21:36.317365 aimsgb-0.1.3/aimsgb/
--rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-0.1.3/aimsgb/__init__.py
--rw-r--r--   0 jianli     (501) staff       (20)     7081 2023-05-23 20:48:44.000000 aimsgb-0.1.3/aimsgb/agb.py
--rw-r--r--   0 jianli     (501) staff       (20)     9250 2023-05-23 20:48:44.000000 aimsgb-0.1.3/aimsgb/grain.py
--rw-r--r--   0 jianli     (501) staff       (20)    22091 2023-05-15 17:32:21.000000 aimsgb-0.1.3/aimsgb/grain_bound.py
--rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-0.1.3/aimsgb/utils.py
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-23 21:21:36.319633 aimsgb-0.1.3/aimsgb.egg-info/
--rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)      310 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/SOURCES.txt
--rw-r--r--   0 jianli     (501) staff       (20)        1 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/dependency_links.txt
--rw-r--r--   0 jianli     (501) staff       (20)       43 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/entry_points.txt
--rw-r--r--   0 jianli     (501) staff       (20)       22 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/requires.txt
--rw-r--r--   0 jianli     (501) staff       (20)        7 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/top_level.txt
--rw-r--r--   0 jianli     (501) staff       (20)       80 2023-05-23 21:21:36.320695 aimsgb-0.1.3/setup.cfg
--rw-r--r--   0 jianli     (501) staff       (20)     5238 2023-05-23 21:20:02.000000 aimsgb-0.1.3/setup.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.827274 aimsgb-1.0.0/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.794040 aimsgb-1.0.0/.github/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.800720 aimsgb-1.0.0/.github/workflows/
+-rw-r--r--   0 jianli     (501) staff       (20)     1113 2023-06-25 21:15:52.000000 aimsgb-1.0.0/.github/workflows/testing.yml
+-rw-r--r--   0 jianli     (501) staff       (20)     1248 2022-06-20 18:41:58.000000 aimsgb-1.0.0/.gitignore
+-rw-r--r--   0 jianli     (501) staff       (20)     1792 2018-10-27 01:29:57.000000 aimsgb-1.0.0/COPYRIGHT.rst
+-rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-1.0.0/LICENSE.txt
+-rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-06-26 04:05:56.827466 aimsgb-1.0.0/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-1.0.0/README.rst
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.805583 aimsgb-1.0.0/aimsgb/
+-rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-1.0.0/aimsgb/__init__.py
+-rw-r--r--   0 jianli     (501) staff       (20)     7053 2023-06-23 20:14:13.000000 aimsgb-1.0.0/aimsgb/agb.py
+-rw-r--r--   0 jianli     (501) staff       (20)    13485 2023-06-26 04:00:50.000000 aimsgb-1.0.0/aimsgb/grain.py
+-rw-r--r--   0 jianli     (501) staff       (20)    22270 2023-06-23 20:14:13.000000 aimsgb-1.0.0/aimsgb/grain_bound.py
+-rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-1.0.0/aimsgb/utils.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.809517 aimsgb-1.0.0/aimsgb.egg-info/
+-rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-06-26 04:05:56.000000 aimsgb-1.0.0/aimsgb.egg-info/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)      836 2023-06-26 04:05:56.000000 aimsgb-1.0.0/aimsgb.egg-info/SOURCES.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        1 2023-06-26 04:05:56.000000 aimsgb-1.0.0/aimsgb.egg-info/dependency_links.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       43 2023-06-26 04:05:56.000000 aimsgb-1.0.0/aimsgb.egg-info/entry_points.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       29 2023-06-26 04:05:56.000000 aimsgb-1.0.0/aimsgb.egg-info/requires.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       24 2023-06-26 04:05:56.000000 aimsgb-1.0.0/aimsgb.egg-info/top_level.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       80 2023-06-26 04:05:56.828156 aimsgb-1.0.0/setup.cfg
+-rw-r--r--   0 jianli     (501) staff       (20)     5191 2023-06-25 21:15:52.000000 aimsgb-1.0.0/setup.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.810111 aimsgb-1.0.0/tests/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.810797 aimsgb-1.0.0/tests/input/
+-rw-r--r--   0 jianli     (501) staff       (20)      356 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/input/POSCAR_mp-13
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.814654 aimsgb-1.0.0/tests/non_cubic/
+-rw-r--r--   0 jianli     (501) staff       (20)      578 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)      577 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)     1606 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)     3068 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)      858 2023-06-25 21:15:52.000000 aimsgb-1.0.0/tests/test_grain.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.822567 aimsgb-1.0.0/tests/time/
+-rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/POSCAR_a
+-rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/POSCAR_b
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.823462 aimsgb-1.0.0/tests/time/out/
+-rw-r--r--   0 jianli     (501) staff       (20)    44157 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/out/POSCAR
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-06-26 04:05:56.826579 aimsgb-1.0.0/tests/time/poscars/
+-rw-r--r--   0 jianli     (501) staff       (20)     1090 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/poscars/POSCAR_MASnI3
+-rw-r--r--   0 jianli     (501) staff       (20)      498 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/poscars/POSCAR_SrTiO3
+-rw-r--r--   0 jianli     (501) staff       (20)      919 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/poscars/POSCAR_TiO2_Anatase
+-rw-r--r--   0 jianli     (501) staff       (20)       44 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/readme.txt
+-rw-r--r--   0 jianli     (501) staff       (20)      975 2023-06-23 20:14:24.000000 aimsgb-1.0.0/tests/time/time.py
```

### Comparing `aimsgb-0.1.3/LICENSE.txt` & `aimsgb-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.3/PKG-INFO` & `aimsgb-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 0.1.3
+Version: 1.0.0
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
```

### Comparing `aimsgb-0.1.3/README.rst` & `aimsgb-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.3/aimsgb/agb.py` & `aimsgb-1.0.0/aimsgb/agb.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,17 +43,16 @@
     if initial_struct is None:
         raise ValueError("Please provide either filename or mpid.")
     
     gb = GrainBoundary(axis, args.sigma, plane, initial_struct, args.uc_a, args.uc_b)
     to_primitive = False if args.conventional else True
     gb.build_gb(args.vacuum, args.add_if_dist, to_primitive, args.delete_layer,
                 args.tol).to(filename=args.out, fmt=args.fmt)
-    print("CSL Matrix (det=%.1f):\n%s" % (np.linalg.det(gb.csl), gb.csl))
-    print("%s of sigma%s[%s]/(%s) is created"
-          % (args.out, gb.sigma, args.axis, gb.plane_str))
+    print(f"CSL Matrix (det={np.linalg.det(gb.csl)}):\n{gb.csl}")
+    print(f"{args.out} of sigma{gb.sigma}[{args.axis}]/({gb.plane_str}) is created")
 
 
 def main():
     parser = argparse.ArgumentParser(description=aimsgb_descript,
                                      formatter_class=argparse.RawTextHelpFormatter)
     subparsers = parser.add_subparsers(help="command", dest="command")
```

### Comparing `aimsgb-0.1.3/aimsgb/grain.py` & `aimsgb-1.0.0/aimsgb/grain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import re
 import warnings
 import numpy as np
+from numpy import sin, radians
 from functools import reduce
 from itertools import groupby
 from aimsgb.utils import reduce_vector
 from pymatgen.core.structure import Structure, Lattice, PeriodicSite
 from pymatgen.transformations.advanced_transformations import CubicSupercellTransformation
 from pymatgen.analysis.structure_matcher import StructureMatcher
 
@@ -56,14 +58,35 @@
             A structure object.
         """
         from mp_api.client import MPRester
 
         mpr = MPRester()
         s = mpr.get_structure_by_material_id(mp_id, conventional_unit_cell=True)
         return cls.from_dict(s.as_dict())
+    
+    def add_selective_dynamics(self, fix_list, tol=0.25, axis=2):
+        """
+        Add selective dynamics properties for sites sorted by layers
+        Args:
+            fix_list (list): A list of layer indices
+            tol (float): Tolerance factor in Angstrom to determnine if sites are 
+                in the same layer. Default to 0.25.
+
+        Returns: A Structure object with selective dynamics properties
+
+        """
+        layers = self.sort_sites_in_layers(tol=tol, axis=axis)
+        sd_sites = []
+        for i, l in enumerate(layers):
+            if i in fix_list:
+                sd_sites.extend(zip([[False, False, False]] * len(l), [_i[1] for _i in l]))
+            else:
+                sd_sites.extend(zip([[True, True, True]] * len(l), [_i[1] for _i in l]))
+        values = [i[0] for i in sorted(sd_sites, key=lambda x: x[1])]
+        self.add_site_property("selective_dynamics", values)
 
     def make_supercell(self, scaling_matrix):
         """
         Create a supercell. Very similar to pymatgen's Structure.make_supercell
         However, we need to make sure that all fractional coordinates that equal
         to 1 will become 0 and the lattice are redefined so that x_c = [0, 0, c]
     
@@ -87,84 +110,84 @@
 
     def delete_bt_layer(self, bt, tol=0.25, axis=2):
         """
         Delete bottom or top layer of the structure.
         Args:
             bt (str): Specify whether it's a top or bottom layer delete. "b"
                 means bottom layer and "t" means top layer.
-            tol (float), Angstrom: Tolerance factor to determine whether two
-                atoms are at the same plane.
-                Default to 0.25
+            tol (float): Tolerance factor in Angstrom to determnine if sites are 
+                in the same layer. Default to 0.25.
             axis (int): The direction of top and bottom layers. 0: x, 1: y, 2: z
 
         """
         if bt == "t":
             l1, l2 = (-1, -2)
         else:
             l1, l2 = (0, 1)
 
         l = self.lattice.abc[axis]
         layers = self.sort_sites_in_layers(tol=tol, axis=axis)
-        l_dist = abs(layers[l1][0].coords[axis] - layers[l2][0].coords[axis])
+        l_dist = abs(layers[l1][0][0].coords[axis] - layers[l2][0][0].coords[axis])
         l_vector = [1, 1]
         l_vector.insert(axis, (l - l_dist) / l)
         new_lat = Lattice(self.lattice.matrix * np.array(l_vector)[:, None])
 
         layers.pop(l1)
         sites = reduce(lambda x, y: np.concatenate((x, y), axis=0), layers)
         new_sites = []
         l_dist = 0 if bt == "t" else l_dist
         l_vector = [0, 0]
         l_vector.insert(axis, l_dist)
-        for i in sites:
-            new_sites.append(PeriodicSite(i.specie, i.coords - l_vector,
+        for site, _ in sites:
+            new_sites.append(PeriodicSite(site.specie, site.coords - l_vector,
                                           new_lat, coords_are_cartesian=True))
         self._sites = new_sites
         self._lattice = new_lat
 
     def sort_sites_in_layers(self, tol=0.25, axis=2):
         """
         Sort the sites in a structure layer by layer.
 
         Args:
-            tol (float): tolerance factor when determine whether two atoms are
-                are at the same plane. Angstrom
+            tol (float): Tolerance factor in Angstrom to determnine if sites are 
+                in the same layer. Default to 0.25.
             axis (int): The direction of top and bottom layers. 0: x, 1: y, 2: z
 
         Returns:
-            Lists with the sites in the same plane as one list.
+            Lists with a list of (site, index) in the same plane as one list.
         """
-        new_atoms = sorted(self, key=lambda x: x.frac_coords[axis])
+        sites_indices = sorted(zip(self.sites, range(len(self))), 
+                               key=lambda x: x[0].frac_coords[axis])
         layers = []
-        for k, g in groupby(new_atoms, key=lambda x: x.frac_coords[axis]):
+        for k, g in groupby(sites_indices, key=lambda x: x[0].frac_coords[axis]):
             layers.append(list(g))
         new_layers = []
         k = -1
         for i in range(len(layers)):
             if i > k:
                 tmp = layers[i]
                 for j in range(i + 1, len(layers)):
                     if self.lattice.abc[axis] * abs(
-                                    layers[j][0].frac_coords[axis] -
-                                    layers[i][0].frac_coords[axis]) < tol:
+                                    layers[j][0][0].frac_coords[axis] -
+                                    layers[i][0][0].frac_coords[axis]) < tol:
                         tmp.extend(layers[j])
                         k = j
                     else:
                         break
                 new_layers.append(sorted(tmp))
         # check if the 1st layer and last layer are actually the same layer
         # use the fractional as cartesian doesn't work for unorthonormal
         if self.lattice.abc[axis] * abs(
-                                new_layers[0][0].frac_coords[axis] + 1 -
-                                new_layers[-1][0].frac_coords[axis]) < tol:
+                                new_layers[0][0][0].frac_coords[axis] + 1 -
+                                new_layers[-1][0][0].frac_coords[axis]) < tol:
             tmp = new_layers[0] + new_layers[-1]
             new_layers = new_layers[1:-1]
             new_layers.append(sorted(tmp))
         return new_layers
-
+    
     def set_orthogonal_grain(self):
         a, b, c = self.lattice.abc
         self.lattice = Lattice.orthorhombic(a, b, c)
 
     def build_grains(self, csl, gb_direction, uc_a=1, uc_b=1):
         """
         Build structures for grain A and B from CSL matrix, number of unit cell
@@ -222,7 +245,67 @@
         scale_vector = [1, 1]
         scale_vector.insert(gb_direction, uc_a)
         grain_a.make_supercell(scale_vector)
 
         # grain_b.to(filename='POSCAR')
         # exit(0)
         return grain_a, grain_b
+
+    @classmethod
+    def stack_grains(cls, grain_a, grain_b, vacuum=0.0, gap=0.0, direction=2,
+                     delete_layer="0b0t0b0t", tol=0.25, to_primitive=True):
+        """
+        Build an interface structure by stacking two grains along a given direction.
+        The grain_b a- and b-vectors will be forced to be the grain_a's
+        a- and b-vectors.
+        Args:
+            grain_a (Grain): Substrate for the interface structure
+            grain_b (Grain): Film for the interface structure
+            vacuum (float): Vacuum space above the film in Angstroms. Default to 0.0
+            gap (float): Gap between substrate and film in Angstroms. Default to 0.0
+            direction (int): Stacking direction of the interface structure. 0: x, 1: y, 2: z.
+            delete_layer (str): Delete top and bottom layers of the substrate and film.
+                8 characters in total. The first 4 characters is for the substrate and
+                the other 4 is for the film. "b" means bottom layer and "t" means
+                top layer. Integer represents the number of layers to be deleted.
+                Default to "0b0t0b0t", which means no deletion of layers. The
+                direction of top and bottom layers is based on the given direction.
+            tol (float): Tolerance factor in Angstrom to determnine if sites are 
+                in the same layer. Default to 0.25.
+            to_primitive (bool): Whether to get primitive structure of GB. Default to true.
+        Returns:
+             GB structure (Grain)
+        """
+        delete_layer = delete_layer.lower()
+        delete = re.findall('(\d+)(\w)', delete_layer)
+        if len(delete) != 4:
+            raise ValueError(f"'{delete_layer}' is not supported. Please make sure the format "
+                             "is 0b0t0b0t.")
+        for i, v in enumerate(delete):
+            for j in range(int(v[0])):
+                if i <= 1:
+                    grain_a.delete_bt_layer(v[1], tol, direction)
+                else:
+                    grain_b.delete_bt_layer(v[1], tol, direction)
+        abc_a = list(grain_a.lattice.abc)
+        abc_b, angles = np.reshape(grain_b.lattice.parameters, (2, 3))
+        if direction == 1:
+            l = (abc_a[direction] + gap) * sin(radians(angles[2]))
+        else:
+            l = abc_a[direction] + gap
+        abc_a[direction] += abc_b[direction] + 2 * gap + vacuum
+        new_lat = Lattice.from_parameters(*abc_a, *angles)
+        a_fcoords = new_lat.get_fractional_coords(grain_a.cart_coords)
+
+        grain_a = Grain(new_lat, grain_a.species, a_fcoords, site_properties=grain_a.site_properties)
+        l_vector = [0, 0]
+        l_vector.insert(direction, l)
+        b_fcoords = new_lat.get_fractional_coords(
+            grain_b.cart_coords + l_vector)
+        grain_b = Grain(new_lat, grain_b.species, b_fcoords, site_properties=grain_b.site_properties)
+
+        structure = Grain.from_sites(grain_a[:] + grain_b[:])
+        structure = structure.get_sorted_structure()
+        if to_primitive:
+            structure = structure.get_primitive_structure()
+
+        return cls.from_dict(structure.as_dict())
```

### Comparing `aimsgb-0.1.3/aimsgb/grain_bound.py` & `aimsgb-1.0.0/aimsgb/grain_bound.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         u2 = y2_1 / norm(y2_1)
         y3 = csl[0] - np.dot(csl[0], u1) * u1 - np.dot(csl[0], u2) * u2
         csl[1] = c0_1
         csl[0] = get_integer(y3)
     for i in range(3):
         for j in range(i + 1, 3):
             if not np.allclose(np.dot(csl[i], csl[j]), 0):
-                raise ValueError("Non-orthogonal basis: %s" % csl)
+                raise ValueError(f"Non-orthogonal basis: {csl}")
     return csl.round().astype(int)
 
 
 class GBInformation(dict):
     """
     GBInformation object essentially consists of a dictionary with information
     including sigma, CSL matrix, GB plane, rotation angle and rotation matrix
@@ -248,37 +248,37 @@
         self.axis = axis
         self.max_sigma = max_sigma
         self.specific = specific
         self.update(self.get_gb_info())
 
     def __str__(self):
         axis_str = "".join(map(str, self.axis))
-        outs = ["Grain boundary information for rotation axis: %s" % axis_str,
-                "Show the sigma values up to %s (Note: * means twist GB)"
-                % (self.max_sigma)]
+        outs = [f"Grain boundary information for rotation axis: {axis_str}",
+                f"Show the sigma values up to {self.max_sigma} (Note: * means twist GB, Theta is the rotation angle)"
+                ]
         data = []
-        to_s = lambda x: "%.2f" % x
+        to_s = lambda x: f"{x:.2f}"
         for key, item in sorted(self.items()):
-            for i, value in enumerate(item["plane"]):
+            for i, value in enumerate(item["GB plane"]):
                 count = -1
                 for v in value:
                     count += 1
-                    plane_str = " ".join(map(str, v))
+                    plane_str = f"({' '.join(map(str, v))})"
                     if v == list(self.axis):
                         plane_str += "*"
                     if count == 0:
-                        row = [key, to_s(self[key]["theta"][i])]
+                        row = [key, to_s(self[key]["Theta"][i])]
                     else:
                         row = [None, None]
                     csl = [" ".join('%2s' % k for k in j)
-                           for j in self[key]["csl"][i]]
-                    row.extend(["(%s)" % plane_str, csl[count]])
+                           for j in self[key]["CSL matrix"][i]]
+                    row.extend([plane_str, csl[count]])
                     data.append(row)
         outs.append(tabulate(data, numalign="center", tablefmt='orgtbl',
-                             headers=["Sigma", "Theta", "GB Plane", "CSL"]))
+                             headers=["Sigma", "Theta", "GB plane", "CSL matrix"]))
         return "\n".join(outs)
 
     def get_gb_info(self):
         """
         Calculate sigma, rotation angle, GB plane, rotation matrix and CSL matrix
         The algorithm for getting sigma, m, n, theta is from H. Grimmer:
         https://doi.org/10.1107/S0108767384000246
@@ -300,15 +300,15 @@
                 if not sigma or sigma > self.max_sigma:
                     continue
                 theta = self.get_theta(m, n)
                 sigma_theta[sigma].append([theta, m, n])
 
         if not sigma_theta:
             raise ValueError("Cannot find any matching GB. Most likely there "
-                             "is no sigma %s%s GB." % (self.max_sigma, self.axis))
+                             f"is no sigma {self.max_sigma}{self.axis} GB.")
         for sigma in sigma_theta:
             sigma_theta[sigma] = sorted(sigma_theta[sigma], key=lambda t: t[0])
             min_theta = sigma_theta[sigma][0][0]
             rot_matrix = self.get_rotate_matrix(min_theta)
             csl_matrix = self.get_csl_matrix(sigma, rot_matrix)
             csl = orthogonalize_csl(csl_matrix, self.axis)
             # Sometime when getting CSL from O-lattice, det not equals to sigma.
@@ -328,23 +328,23 @@
                                 ext_csl[i] = [v[0] / abs(v[0]) * n, v[1] / abs(v[1]) * m, 0]
                     if (csl == ext_csl).all():
                         ind += 1
                     else:
                         break
                 all_csl = [csl, ext_csl]
                 if ind:
-                    gb_info[sigma] = {"theta": [min_theta, 90 - min_theta]}
+                    gb_info[sigma] = {"Theta": [min_theta, 90 - min_theta]}
                 else:
-                    gb_info[sigma] = {"theta": [90 - min_theta, min_theta]}
+                    gb_info[sigma] = {"Theta": [90 - min_theta, min_theta]}
             else:
-                gb_info[sigma] = {"theta": [min_theta]}
+                gb_info[sigma] = {"Theta": [min_theta]}
 
-            gb_info[sigma].update({"plane": [[list(j) for j in i.transpose()]
+            gb_info[sigma].update({"GB plane": [[list(j) for j in i.transpose()]
                                              for i in all_csl],
-                                   "rot_matrix": rot_matrix, "csl": all_csl})
+                                   "Rotation matrix": rot_matrix, "CSL matrix": all_csl})
         return gb_info
 
     def get_theta(self, m, n):
         """
         Calculate rotation angle from m, n
 
         Args:
@@ -446,16 +446,16 @@
         self.axis = axis
         self.plane = list(plane)
         self.plane_str = " ".join(map(str, self.plane))
 
         if sigma % 2 == 0:
             reduce_sigma = reduce_integer(sigma)
             warnings.warn(
-                "{} is an even number. However sigma must be an odd number. "
-                "We will choose sigma={}.".format(sigma, reduce_sigma),
+                f"{sigma} is an even number. However sigma must be an odd number. "
+                f"We will choose sigma={reduce_sigma}.",
                 RuntimeWarning)
             sigma = reduce_sigma
         self.sigma = sigma
         self.gb_info = GBInformation(self.axis, self.sigma, specific=True)
         self.gb_direction = None
         for i, v in enumerate(self.csl.transpose()):
             if self.plane == list(v):
@@ -467,36 +467,36 @@
             self.csl, self.gb_direction, uc_a, uc_b)
 
     @property
     def rot_matrix(self):
         """
         Rotation matrix for calculating CSL matrix
         """
-        return self.gb_info[self.sigma]["rot_matrix"]
+        return self.gb_info[self.sigma]["Rotation matrix"]
 
     @property
     def theta(self):
         """
         Rotation angle for calculating rotation matrix and to bring two grains
         into a perfect match
         """
-        return self.gb_info[self.sigma]["theta"]
+        return self.gb_info[self.sigma]["Theta"]
 
     @property
     def csl(self):
         """
         CSL matrix
         """
-        for i, v in enumerate(self.gb_info[self.sigma]["plane"]):
+        for i, v in enumerate(self.gb_info[self.sigma]["GB plane"]):
             if self.plane in v:
-                return self.gb_info[self.sigma]["csl"][i]
+                return self.gb_info[self.sigma]["CSL matrix"][i]
         avail_plane = ", ".join([", ".join([" ".join(map(str, j)) for j in i])
-                                 for i in self.gb_info[self.sigma]["plane"]])
-        raise ValueError("The given GB plane '%s' cannot be realized. Choose "
-                         "the plane in [%s]" % (self.plane_str, avail_plane))
+                                 for i in self.gb_info[self.sigma]["GB plane"]])
+        raise ValueError(f"The given GB plane '{self.plane_str}' cannot be realized. Choose "
+                         f"the plane in [{avail_plane}]")
 
     @property
     def grain_a(self):
         """
         Grain class instance for grain A
         """
         return self._grain_a
@@ -529,19 +529,21 @@
                 direction of top and bottom layers is based on gb_direction.
             tol (float), Angstrom: Tolerance factor to determine whether two
                 atoms are at the same plane.
                 Default to 0.25
         Returns:
              GB structure (Grain)
         """
+        warnings.warn("The build_gb method is deprecated. Please use Grain.stack_grains methode instead.")
+        
         ind = self.gb_direction
         delete_layer = delete_layer.lower()
         delete = re.findall('(\d+)(\w)', delete_layer)
         if len(delete) != 4:
-            raise ValueError("'%s' is not supported. Please make sure the format "
+            raise ValueError(f"'{delete_layer}' is not supported. Please make sure the format "
                              "is 0b0t0b0t.")
         for i, v in enumerate(delete):
             for j in range(int(v[0])):
                 if i <= 1:
                     self.grain_a.delete_bt_layer(v[1], tol, ind)
                 else:
                     self.grain_b.delete_bt_layer(v[1], tol, ind)
```

### Comparing `aimsgb-0.1.3/aimsgb/utils.py` & `aimsgb-1.0.0/aimsgb/utils.py`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.3/aimsgb.egg-info/PKG-INFO` & `aimsgb-1.0.0/aimsgb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 0.1.3
+Version: 1.0.0
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
```

### Comparing `aimsgb-0.1.3/setup.py` & `aimsgb-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 
 long_desc = """
 Introduction
 ============
 aimsgb, an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
 construct various grain boundary structures from cubic and non-cubic initial
@@ -75,35 +75,33 @@
 About the aimsgb Development Team
 =================================
 http://materials.ucsd.edu/
 """
 
 setup(
     name="aimsgb",
-    packages=find_packages(),
-    version="0.1.3",
+    packages=find_namespace_packages(exclude=["*.tests"]),
+    version="1.0.0",
     setup_requires=["setuptools>=18.0"],
-    install_requires=["pymatgen", "mp_api", "numpy"],
+    install_requires=["pymatgen", "mp_api", "numpy", "pytest"],
     include_package_data=True,
     author="Jianli Cheng and Kesong YANG",
     maintainer="Jianli Cheng, Sicong JIANG, and Kesong YANG",
     maintainer_email="chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu",
     url="http://aimsgb.org",
     description="aimsgb is a python library for generatng the atomic "
                 "coordinates of periodic grain boundaries."
                 "Copyright © 2018 The Regents of the University of California."
                 "All Rights Reserved. See more in Copyright.",
     long_description=long_desc,
     keywords=["material science", "grain boundary", "molecular simulation"],
     classifiers=[
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
```

