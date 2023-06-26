# Comparing `tmp/pycoxmunk-1.0.0.tar.gz` & `tmp/pycoxmunk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycoxmunk-1.0.0.tar", last modified: Tue Nov  8 15:02:19 2022, max compression
+gzip compressed data, was "pycoxmunk-1.1.0.tar", last modified: Mon Jun 26 09:57:15 2023, max compression
```

## Comparing `pycoxmunk-1.0.0.tar` & `pycoxmunk-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-11-08 15:02:19.521095 pycoxmunk-1.0.0/
--rw-rw-rw-   0        0        0    35823 2022-08-05 14:59:51.000000 pycoxmunk-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    44774 2022-11-08 15:02:19.521095 pycoxmunk-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2874 2022-11-08 14:48:47.000000 pycoxmunk-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-08 15:02:19.503095 pycoxmunk-1.0.0/pycoxmunk/
--rw-rw-rw-   0        0        0    22962 2022-11-08 12:55:23.000000 pycoxmunk-1.0.0/pycoxmunk/CM_Calcs.py
--rw-rw-rw-   0        0        0     7652 2022-11-03 15:16:52.000000 pycoxmunk-1.0.0/pycoxmunk/CM_Constants.py
--rw-rw-rw-   0        0        0    13259 2022-11-07 14:51:49.000000 pycoxmunk-1.0.0/pycoxmunk/CM_Main.py
--rw-rw-rw-   0        0        0     3460 2022-10-14 09:31:48.000000 pycoxmunk-1.0.0/pycoxmunk/CM_PixMask.py
--rw-rw-rw-   0        0        0    12454 2022-11-07 14:30:53.000000 pycoxmunk-1.0.0/pycoxmunk/CM_SceneGeom.py
--rw-rw-rw-   0        0        0     6764 2022-10-19 12:13:57.000000 pycoxmunk-1.0.0/pycoxmunk/CM_Shared_Wind.py
--rw-rw-rw-   0        0        0     4264 2022-11-03 11:58:43.000000 pycoxmunk-1.0.0/pycoxmunk/CM_Utils.py
-drwxrwxrwx   0        0        0        0 2022-11-08 15:02:19.508094 pycoxmunk-1.0.0/pycoxmunk/Tests/
--rw-rw-rw-   0        0        0        0 2022-08-05 14:59:51.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/__init__.py
--rw-rw-rw-   0        0        0    11399 2022-10-17 15:56:35.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_CMCalcs.py
--rw-rw-rw-   0        0        0    13452 2022-11-08 12:46:40.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_CM_main.py
--rw-rw-rw-   0        0        0     2522 2022-10-04 14:30:29.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_PixMask.py
--rw-rw-rw-   0        0        0     8335 2022-10-19 12:08:23.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_SceneGeom.py
--rw-rw-rw-   0        0        0     3159 2022-08-05 15:01:18.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_SharedWind.py
--rw-rw-rw-   0        0        0     3608 2022-10-07 12:30:08.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_Utils.py
--rw-rw-rw-   0        0        0     2617 2022-08-05 15:01:18.000000 pycoxmunk-1.0.0/pycoxmunk/Tests/test_WaterConsts.py
--rw-rw-rw-   0        0        0      915 2022-10-10 14:53:18.000000 pycoxmunk-1.0.0/pycoxmunk/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-08 15:02:19.519094 pycoxmunk-1.0.0/pycoxmunk.egg-info/
--rw-rw-rw-   0        0        0    44774 2022-11-08 15:02:19.000000 pycoxmunk-1.0.0/pycoxmunk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2022-11-08 15:02:19.000000 pycoxmunk-1.0.0/pycoxmunk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-08 15:02:19.000000 pycoxmunk-1.0.0/pycoxmunk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2022-11-08 15:02:19.000000 pycoxmunk-1.0.0/pycoxmunk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-08 15:02:19.000000 pycoxmunk-1.0.0/pycoxmunk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1004 2022-11-08 15:02:11.000000 pycoxmunk-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      950 2022-11-08 15:02:19.523094 pycoxmunk-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:15.016663 pycoxmunk-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2022-08-05 14:59:51.000000 pycoxmunk-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4243 2023-06-26 09:57:15.016663 pycoxmunk-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3553 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:15.006663 pycoxmunk-1.1.0/pycoxmunk/
+-rw-rw-rw-   0        0        0    22898 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_Calcs.py
+-rw-rw-rw-   0        0        0     7533 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_Constants.py
+-rw-rw-rw-   0        0        0    13188 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_Main.py
+-rw-rw-rw-   0        0        0     3396 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_PixMask.py
+-rw-rw-rw-   0        0        0    12388 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_SceneGeom.py
+-rw-rw-rw-   0        0        0     6700 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_Shared_Wind.py
+-rw-rw-rw-   0        0        0     4200 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/CM_Utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:15.010664 pycoxmunk-1.1.0/pycoxmunk/Tests/
+-rw-rw-rw-   0        0        0        0 2022-08-05 14:59:51.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/__init__.py
+-rw-rw-rw-   0        0        0    12187 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_CMCalcs.py
+-rw-rw-rw-   0        0        0    15631 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_CM_main.py
+-rw-rw-rw-   0        0        0     2414 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_PixMask.py
+-rw-rw-rw-   0        0        0     9924 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_SceneGeom.py
+-rw-rw-rw-   0        0        0     3182 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_SharedWind.py
+-rw-rw-rw-   0        0        0     3462 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_Utils.py
+-rw-rw-rw-   0        0        0     2410 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/Tests/test_WaterConsts.py
+-rw-rw-rw-   0        0        0      859 2023-06-26 09:36:24.000000 pycoxmunk-1.1.0/pycoxmunk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:15.014663 pycoxmunk-1.1.0/pycoxmunk.egg-info/
+-rw-rw-rw-   0        0        0     4243 2023-06-26 09:57:14.000000 pycoxmunk-1.1.0/pycoxmunk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-06-26 09:57:14.000000 pycoxmunk-1.1.0/pycoxmunk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:57:14.000000 pycoxmunk-1.1.0/pycoxmunk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-06-26 09:57:14.000000 pycoxmunk-1.1.0/pycoxmunk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 09:57:14.000000 pycoxmunk-1.1.0/pycoxmunk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1002 2023-06-26 09:36:45.000000 pycoxmunk-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      950 2023-06-26 09:57:15.017663 pycoxmunk-1.1.0/setup.cfg
```

### Comparing `pycoxmunk-1.0.0/LICENSE` & `pycoxmunk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycoxmunk-1.0.0/README.md` & `pycoxmunk-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,33 @@
 
 It is also available from `conda-forge` for conda installations:
 
 ```bash
     conda install -c conda-forge pycoxmunk
 ```
 
+Tests
+-----
+
+pycoxmunk comes with a set of scripts for testing the functionality of the library. These are located in the `./Tests/`
+subdirectory and can be run using `pytest`:
+
+```
+
+cd Tests
+pytest .
+
+```
+
+This will run all tests. You can also run just a single test script with, for example, `pytest test_CMCalcs.py`.
+You may first need to install pytest via: `conda install pytest`.
+
+Once testing is complete, a summary will be displayed. This should indicate that all tests have passed, as well as
+potentially listing some warnings depending on your environment and the current status of `pycoxmunk`'s dependencies.
+
 Credits
 -------
 
 This code was written by Simon Proud and is based on a fortran implementation of the Cox-Munk algorithm written by 
 Greg McGarragh as part of the [ORAC algorithm](https://github.com/ORAC-CC/orac).
 
 Feedback and Contribution
@@ -56,10 +75,11 @@
     from satpy import debug_on
     debug_on()
 ```
 
 This will print additional log and diagnostic information.
 
 Suggestions for new features are welcome, but may not always be possible for me to code due to limited time. You can
-also submit your own [pull requests](https://github.com/simonrp84/PyCoxMunk/pulls) that add features of fix bugs. This is the recommended way to change the library
-code, rather than emailing me your updates. By submitting a pull request your changes are documented and your 
-contribution to the code is clear.
+also submit your own [pull requests](https://github.com/simonrp84/PyCoxMunk/pulls) that add features of fix bugs. 
+This is the recommended way to change the library code, rather than emailing me your updates. 
+By submitting a pull request please ensure that your code changes and additions are documented and, where appropriate, 
+covered by tests.
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_Calcs.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_Calcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_Constants.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_Constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
@@ -35,30 +34,29 @@
                         [2.86324e-3, 1.86059e-3, -4.69589e-4]])
 
 # For the BRDF computations
 n_quad_theta = 4
 n_quad_phi = 4
 
 
-
 class WaterData:
     """A class for data about water at a given wavelength."""
 
     def __init__(self,
-                 wavelength,       # Wavelength of given information
-                 refrac_real,      # Real part of refractive index
-                 refrac_imag,      # Imaginary part of refractive index
-                 base_abs,         # Base water absorption
-                 base_backscat,    # Base water backscatter coefficient
-                 whitecap_refl,    # Reflectance of whitecaps
-                 chl_a_coef,       # Chlorophyll-a absorption coefficient part
-                 total_abs,        # Total water absorption
-                 total_backscat,   # Total water backscatter
-                 chlabs=0,           # Chlorophyll-a absorption
-                 chlbsc=0):          # Chlorophyll-a backscatter
+                 wavelength,  # Wavelength of given information
+                 refrac_real,  # Real part of refractive index
+                 refrac_imag,  # Imaginary part of refractive index
+                 base_abs,  # Base water absorption
+                 base_backscat,  # Base water backscatter coefficient
+                 whitecap_refl,  # Reflectance of whitecaps
+                 chl_a_coef,  # Chlorophyll-a absorption coefficient part
+                 total_abs,  # Total water absorption
+                 total_backscat,  # Total water backscatter
+                 chlabs=0,  # Chlorophyll-a absorption
+                 chlbsc=0):  # Chlorophyll-a backscatter
 
         # Check the chl-a coefficients are a 2-element list
         if type(chl_a_coef) is not list:
             raise TypeError("Chlorophyll-a absorption coefficient should be a 2-element list.")
         if len(chl_a_coef) != 2:
             raise TypeError("Chlorophyll-a absorption coefficient should be a 2-element list.")
         self.wavelength = wavelength
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_Main.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_Main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
@@ -153,15 +152,15 @@
         # Cox Munk output class, used later
         self.cm_refl = CMReflectance()
 
         # Compute longitudes and latitudes from first selected band. Assumes all bands are same
         # dimensions! This means that high res bands (such as Himawari B03) must be resampled to
         # lower res band resolution before passing to PyCoxMunk. If you wish to process both
         # high and low res bands at native resolution then you must call PyCoxMunk multiple times.
-        lons, lats = self.scn[self.band_names[0]].attrs['area'].get_lonlats_dask()
+        lons, lats = self.scn[self.band_names[0]].attrs['area'].get_lonlats()
 
         self.geometry = CMSceneGeom(da.array(self.scn[self.angle_names['sza']]),
                                     da.array(self.scn[self.angle_names['saa']]),
                                     da.array(self.scn[self.angle_names['vza']]),
                                     da.array(self.scn[self.angle_names['vaa']]),
                                     da.array(lats),
                                     da.array(lons))
@@ -213,15 +212,14 @@
             except (NameError, AttributeError):
                 pass
             try:
                 del self.cm_refl.rhowc
             except (NameError, AttributeError):
                 pass
 
-
     def retr_coxmunk_refl(self):
         """Main function for computing the sea surface reflectance.
 
         This uses data previously loaded including, if available, wind and ocean color
         data to compute the reflectance using the approach described in Sayer (2010).
         DOI: 10.5194/amt-3-813-2010
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_PixMask.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_PixMask.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2022 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_SceneGeom.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_SceneGeom.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
@@ -265,15 +264,14 @@
             if da.any(self.raa < self.relazi_min) or da.any(self.raa >= self.relazi_max):
                 raise ValueError("All Relative azimuth angles must be in the range " +
                                  str(self.azimuth_min) + ' to ' + str(self.relazi_max))
             # Convert to float if single value
             if self.raa.shape == () or self.raa.shape == (0,):
                 self.raa = float(self.raa)
 
-
     def calc_relazi(self):
         """Compute the relative azimuth angles from solar and viewing azimuths."""
         raa = da.abs(self.vaa - self.saa)
 
         # If any RAA values are greater than 180, invert them.
         raa = da.where(raa >= 180., 360. - raa, raa)
         return raa
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_Shared_Wind.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_Shared_Wind.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/CM_Utils.py` & `pycoxmunk-1.1.0/pycoxmunk/CM_Utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-
-#!/usr/bin/env python
+# !/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
@@ -84,26 +82,26 @@
     ib = n * (n + 1)
 
     da = (n - 1) / (8. * n ** 3)
 
     db = (x1 + x2) / 2.
     dc = (x2 - x1) / 2.
 
-    ii = int(da_ar.floor(n-1))
+    ii = int(da_ar.floor(n - 1))
     for i in range(0, int(da_ar.floor(nn))):
         y1, p2 = _gauss_leg_point(n, i, ia, ib, da)
 
         dd = dc * y1
 
         x[i] = db - dd
         x[ii] = db + dd
 
         de = n * p2
         de = 2 / (de * de)
-        w[i] = (dc - dd*y1) * de
+        w[i] = (dc - dd * y1) * de
 
         w[ii] = w[i]
 
         ii = ii - 1
 
     return x, w
 
@@ -118,15 +116,15 @@
         raise ValueError("Cannot resize array and sizes do not match.")
     return arr
 
 
 def check_type(in_val, var_typ):
     """Check that input variable is correct type.
     All inputs should be numpy array or a float."""
-    if type(in_val) == float or type(in_val) == np.float64 or type(in_val) == np.float:
+    if type(in_val) == float or type(in_val) == np.float64 or type(in_val) == float:
         return in_val
     elif isinstance(in_val, np.ndarray):
         return da_ar.array(in_val)
     elif isinstance(in_val, xr.DataArray):
         return da_ar.array(in_val)
     elif isinstance(in_val, da_ar.Array):
         return in_val
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/Tests/test_CMCalcs.py` & `pycoxmunk-1.1.0/pycoxmunk/Tests/test_CMCalcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
@@ -21,100 +20,108 @@
 from pycoxmunk.CM_Constants import CM_DATA_DICT, WaterData
 from pycoxmunk.CM_Shared_Wind import CMSharedWind
 from pycoxmunk.CM_SceneGeom import CMSceneGeom
 import pycoxmunk.CM_Calcs as CMCalcs
 from copy import deepcopy
 from unittest import mock
 import numpy as np
-import unittest
 
 
-class TestCMCalcs(unittest.TestCase):
-    def setUp(self):
+class TestCMCalcs:
+    def setup_method(self):
         """Set up some common variables for the tests."""
         self.sza = np.array([58.655, 167.412, 3.173, 63.215])
         self.vza = np.array([57.733, 21.248, 57.777, 99.768])
         self.saa = np.array([285.129, 133.130, 57.125, 223.555])
         self.vaa = np.array([38.505, 185.793, 133.017, 341.330])
         self.raa = np.array([113.376, 52.663, 75.892, 117.775])
         self.lats = np.array([-5.247, -58.473, 17.666, 48.237])
         self.lons = np.array([-116.184, 73.047, 120.744, -121.522])
 
-        self.refl = CMCalcs.CMReflectance(cwvl=0.84,
-                                           rho=np.array([1., 10., 100.]))
+        self.refl = CMCalcs.CMReflectance(cwvl=0.84, rho=np.array([1., 10., 100.]))
         self.watprops = deepcopy(CM_DATA_DICT[0.47])
         self.watprops.chlabs = 0.0109369
         self.watprops.chlbsc = 0.01805958
-        self.geom = CMSceneGeom(self.sza, self.saa, self.vza, self.vaa, self.lats, self.lons)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            self.geom = CMSceneGeom(self.sza, self.saa, self.vza, self.vaa, self.lats, self.lons)
         self.wind = CMSharedWind(self.geom, -5., 1.2)
 
     def test_cmrefl(self):
         """Test the CM_Reflectance class."""
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs.CMReflectance(cwvl='1.3')
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs.CMReflectance(cwvl=1)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs.CMReflectance(cwvl=[1., 2.])
 
         cmref = CMCalcs.CMReflectance(cwvl=1.3)
-        self.assertEqual(1.3, cmref.cwvl)
-        self.assertEqual(None, cmref.rhowc)
+        assert 1.3 == cmref.cwvl
+        assert cmref.rhowc is None
 
         cmref = CMCalcs.CMReflectance(cwvl=1.3, rho=1.54, rhowc=12.3)
-        self.assertEqual(1.54, cmref.rho)
-        self.assertEqual(12.3, cmref.rhowc)
+        assert 1.54 == cmref.rho
+        assert 12.3 == cmref.rhowc
 
     def test_compute_bands(self):
         """Test code that selects Cox-Munk bands."""
         blist = [0.22, 0.47, 0.65, 0.83, 1.4, 1.92, 2.56, 3.4, 4.1]
         ex_res = [(None, 0.47), (None, 0.47), (0.65, 0.87), (0.65, 0.87),
                   (1.375, 1.6), (1.6, 2.13), (2.13, 3.7), (2.13, 3.7), (3.7, None)]
-        for i in range(0, len(blist)):
-            self.assertEqual(CMCalcs._compute_bands_to_use(blist[i]), ex_res[i])
-        with self.assertRaises(ValueError):
+        with pytest.warns(UserWarning,
+                          match="Warning: Band wavelength 0.22 is less than PyCoxMunk minimum wavelength 0.47"):
+            assert CMCalcs._compute_bands_to_use(blist[0]), ex_res[0]
+        with pytest.warns(UserWarning,
+                          match="Warning: Band wavelength 0.47 is less than PyCoxMunk minimum wavelength 0.47"):
+            assert CMCalcs._compute_bands_to_use(blist[1]), ex_res[1]
+        for i in range(2, len(blist) - 1):
+            assert CMCalcs._compute_bands_to_use(blist[i]), ex_res[i]
+        with pytest.warns(UserWarning,
+                          match="Warning: Band wavelength 4.1 is greater than PyCoxMunk maximum wavelength 3.7"):
+            assert CMCalcs._compute_bands_to_use(blist[-1]), ex_res[-1]
+        with pytest.raises(ValueError):
             CMCalcs._compute_bands_to_use(0.18)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs._compute_bands_to_use(5.18)
 
     def test_interp_frac(self):
         """Test interpolation of wavelengths."""
         w1 = 0.45
         w2 = 0.65
         cw = [0.45, 0.47, 0.53, 0.59, 0.64]
         omins = [(1.0, 0.0), (0.9, 0.1), (0.6, 0.4), (0.3, 0.7), (0.05, 0.95)]
         for i in range(0, len(cw)):
             retr = CMCalcs._get_interp_frac(w1, w2, cw[i])
-            self.assertAlmostEqual(retr[0], omins[i][0])
-            self.assertAlmostEqual(retr[1], omins[i][1])
+            np.testing.assert_almost_equal(retr[0], omins[i][0])
+            np.testing.assert_almost_equal(retr[1], omins[i][1])
 
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs._get_interp_frac(1, 2, 0.5)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs._get_interp_frac(1, 2, 2.5)
 
     @mock.patch('pycoxmunk.CM_Calcs._compute_bands_to_use')
     @mock.patch('pycoxmunk.CM_Calcs._get_interp_frac')
     def test_compute_water_wvl(self, interp, band):
         """Test selection of wavelength used for water properties."""
         band_mock = mock.MagicMock()
         interp_mock = mock.MagicMock()
 
         band.return_value = band_mock
         interp.return_value = interp_mock
         # Check error is raised if bad interpolation method is requested
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CMCalcs.compute_wavelength_specific_water_props(0.8, meth='random')
 
         # Check error is raised if no previous band is available
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             band.return_value = (None, 0.9)
             CMCalcs.compute_wavelength_specific_water_props(0.8, meth='prev')
         # Check error is raised if no next band is available
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             band.return_value = (0.9, None)
             CMCalcs.compute_wavelength_specific_water_props(0.8, meth='next')
 
         # Check warning is raised if switching from interp to prev/next method
         with pytest.warns(UserWarning):
             band.return_value = (0.47, None)
             CMCalcs.compute_wavelength_specific_water_props(0.8, meth='interp')
@@ -122,46 +129,45 @@
             band.return_value = (None, 1.375)
             CMCalcs.compute_wavelength_specific_water_props(0.8, meth='interp')
 
         # Check correct data is returned for prev method.
         ret_wvl = 0.47
         band.return_value = (ret_wvl, None)
         ret_data = CMCalcs.compute_wavelength_specific_water_props(0.8, meth='prev')
-        self.assertTrue(type(ret_data) == WaterData)
-        self.assertEqual(ret_data.whitecap_refl, CM_DATA_DICT[ret_wvl].whitecap_refl)
-        self.assertEqual(ret_data.wavelength, CM_DATA_DICT[ret_wvl].wavelength)
+        assert type(ret_data) is WaterData
+        assert ret_data.whitecap_refl, CM_DATA_DICT[ret_wvl].whitecap_refl
+        assert ret_data.wavelength, CM_DATA_DICT[ret_wvl].wavelength
 
         # Check correct data is returned for next method.
         ret_wvl = 1.375
         band.return_value = (None, ret_wvl)
         ret_data = CMCalcs.compute_wavelength_specific_water_props(0.8, meth='next')
-        self.assertTrue(type(ret_data) == WaterData)
-        self.assertEqual(ret_data.whitecap_refl, CM_DATA_DICT[ret_wvl].whitecap_refl)
-        self.assertEqual(ret_data.wavelength, CM_DATA_DICT[ret_wvl].wavelength)
+        assert type(ret_data) is WaterData
+        assert ret_data.whitecap_refl, CM_DATA_DICT[ret_wvl].whitecap_refl
+        assert ret_data.wavelength, CM_DATA_DICT[ret_wvl].wavelength
 
         # Check interp works correctly
         frac1 = 0.3
         frac2 = 0.7
         band1 = 0.65
         band2 = 0.87
         interp.return_value = (frac1, frac2)
         band.return_value = (band1, band2)
         ret_data = CMCalcs.compute_wavelength_specific_water_props(0.8, meth='interp')
-        self.assertEqual(ret_data.wavelength, 0.8)
-        self.assertEqual(ret_data.base_abs,
-                         CM_DATA_DICT[band1].base_abs * frac1 + CM_DATA_DICT[band2].base_abs * frac2)
-        self.assertEqual(ret_data.whitecap_refl,
-                         CM_DATA_DICT[band1].whitecap_refl * frac1 + CM_DATA_DICT[band2].whitecap_refl * frac2)
+        assert ret_data.wavelength == 0.8
+        assert ret_data.base_abs == CM_DATA_DICT[band1].base_abs * frac1 + CM_DATA_DICT[band2].base_abs * frac2
+        assert ret_data.whitecap_refl == (CM_DATA_DICT[band1].whitecap_refl * frac1
+                                          + CM_DATA_DICT[band2].whitecap_refl * frac2)
 
     def test_oceancolor(self):
         """Test the ocean color calculations. Functionality currently very basic in the main code."""
         from copy import deepcopy
 
         # Test we raise error if OC data is supplied, as we don't support it yet.
-        with self.assertRaises(NotImplementedError):
+        with pytest.raises(NotImplementedError):
             CMCalcs.run_oceancolor(None, 'a string')
 
         # Test that correct data is returned for chlorophyll.
         expected = (0.0109369, 0.01805958)
         in_data = deepcopy(CM_DATA_DICT[0.47])
         in_data.whitecap_refl = 50
         out_data = CMCalcs.run_oceancolor(in_data)
@@ -187,25 +193,30 @@
 
     def test_calc_coxmunk_brdf(self):
         """Test calculation of the Cox-Munk BRDF parameters."""
         mock_wind = mock.MagicMock()
         mock_wind.u10 = np.array([10.])
         mock_wind.v10 = np.array([-2.1])
         geom = CMSceneGeom(10., np.array([[165.2, 123.1, 22.6], [34, 21.2, 170.4], [0.45, 128.89, 44.22]]),
-                           58.23, 9.3, 12., -120.,)
+                           58.23, 9.3, 12., -120., )
 
-        exp_dv = np.array([0.63585471, 0.63585471, 0.63585471])
-        exp_0d = np.array([4.78758539, 4.78758539, 4.78758539])
-        exp_dd = np.array([0.355864, 0.355864, 0.355864])
+        exp_dv = np.array([[1.702098, 1.673689, 1.715214],
+                           [1.706389, 1.715966, 1.707012],
+                           [1.714822, 1.675567, 1.696584]])
+        exp_0d = np.array([[2.389888, 2.282412, 2.424333],
+                           [2.401838, 2.426135, 2.403517],
+                           [2.423389, 2.29209, 2.373374]])
+        exp_dd = np.array([[1.97325, 1.945448, 1.980272],
+                           [1.975696, 1.980641, 1.976037],
+                           [1.98008, 1.948862, 1.969804]])
         res = CMCalcs.calc_cox_munk_brdf_terms(self.refl, 0.8, geom, mock_wind, None)
         np.testing.assert_allclose(self.refl.rho, res.rho_0v)
-        print(f'{res.rho_dd}')
-        #np.testing.assert_allclose(exp_dd, res.rho_dd)
-        #np.testing.assert_allclose(exp_0d, res.rho_0d)
-        #np.testing.assert_allclose(exp_dv, res.rho_dv)
+        np.testing.assert_allclose(exp_dd, res.rho_dd, atol=1e-6)
+        np.testing.assert_allclose(exp_0d, res.rho_0d, atol=1e-6)
+        np.testing.assert_allclose(exp_dv, res.rho_dv, atol=1e-6)
 
     @mock.patch('pycoxmunk.CM_Calcs.compute_wavelength_specific_water_props')
     @mock.patch('pycoxmunk.CM_Calcs.run_oceancolor')
     @mock.patch('pycoxmunk.CM_Calcs._compute_abcd')
     def test_calc_coxmunk(self, abcd, run_oc, watprops):
         """Test the main Cox-Munk calculation."""
 
@@ -228,13 +239,13 @@
     @mock.patch('pycoxmunk.CM_Calcs.calc_cox_munk')
     @mock.patch('pycoxmunk.CM_Calcs.calc_cox_munk_brdf_terms')
     def test_cm_wrapper(self, ccm_brdf, ccm):
         """Test the wrapper function to ensure it makes calls correctly."""
 
         # Case with no BRDF
         CMCalcs.calc_coxmunk_wrapper(None, None, None, None, False)
-        self.assertTrue(ccm.called)
-        self.assertFalse(ccm_brdf.called)
+        assert ccm.called
+        assert not ccm_brdf.called
         # Case with BRDF
         CMCalcs.calc_coxmunk_wrapper(None, None, None, None, True)
-        self.assertTrue(ccm.called)
-        self.assertTrue(ccm_brdf.called)
+        assert ccm.called
+        assert ccm_brdf.called
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/Tests/test_CM_main.py` & `pycoxmunk-1.1.0/pycoxmunk/Tests/test_CM_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,37 +2,35 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
 """Test the Cox-Munk calculations module."""
+import pytest
 from pyresample import create_area_def
 from datetime import datetime
 from pycoxmunk.CM_Main import PyCoxMunk
-from pycoxmunk.CM_PixMask import CMPixMask
 from unittest import mock
 from satpy import Scene
 import dask.array as da
 import xarray as xr
 import numpy as np
-import unittest
 
 
-class TestCMMain(unittest.TestCase):
+class TestCMMain:
     """Tests for the overarching CM_Main module."""
 
     @staticmethod
     def create_test_scene(band_names, angle_names):
 
         # Define orbital parameters used for lat/lon calculation
         orb_par = {'projection_longitude': 0.0,
@@ -54,21 +52,37 @@
             scn[band] = xr.DataArray(da.from_array(np.zeros((10, 10))),
                                      coords={'y': np.zeros(10), 'x': np.zeros(10)},
                                      attrs={'start_time': datetime.utcnow(),
                                             'area': targ_area,
                                             'wavelength': wvl_mock,
                                             'orbital_parameters': orb_par})
 
-        for band in angle_names.keys():
-            scn[angle_names[band]] = xr.DataArray(da.from_array(np.zeros((10, 10))),
-                                                  coords={'y': np.zeros(10), 'x': np.zeros(10)},
-                                                  attrs={'start_time': datetime.utcnow()})
+        if 'sza' in angle_names.keys():
+            np.random.seed(1024)
+            scn['solar_zenith_angle'] = xr.DataArray(da.from_array(np.linspace(0, 89, 100).reshape((10, 10))),
+                                                     coords={'y': np.zeros(10), 'x': np.zeros(10)},
+                                                     attrs={'start_time': datetime.utcnow()})
+        if 'saa' in angle_names.keys():
+            np.random.seed(2048)
+            scn['solar_azimuth_angle'] = xr.DataArray(da.from_array(np.linspace(0, 360, 100).reshape((10, 10))),
+                                                      coords={'y': np.zeros(10), 'x': np.zeros(10)},
+                                                      attrs={'start_time': datetime.utcnow()})
+        if 'vza' in angle_names.keys():
+            np.random.seed(4096)
+            scn['satellite_zenith_angle'] = xr.DataArray(da.from_array(np.linspace(0, 89, 100).reshape((10, 10))),
+                                                         coords={'y': np.zeros(10), 'x': np.zeros(10)},
+                                                         attrs={'start_time': datetime.utcnow()})
+        if 'vaa' in angle_names.keys():
+            np.random.seed(8192)
+            scn['satellite_azimuth_angle'] = xr.DataArray(da.from_array(np.linspace(0, 360, 100).reshape((10, 10))),
+                                                          coords={'y': np.zeros(10), 'x': np.zeros(10)},
+                                                          attrs={'start_time': datetime.utcnow()})
         return scn
 
-    def setUp(self):
+    def setup_method(self):
         self.good_bnd_names = ['VIS006']
         self.missing_angle_names = {'sza': 'solar_zenith_angle',
                                     'vza': 'satellite_zenith_angle',
                                     'saa': 'solar_azimuth_angle'}
 
         self.good_angle_names = self.missing_angle_names.copy()
         self.good_angle_names['vaa'] = 'satellite_azimuth_angle'
@@ -79,98 +93,104 @@
     @staticmethod
     def _get_lonlats():
         return np.array([10, 11]), np.array([5, 6])
 
     def test_badbools(self):
         """Test some of the boolean options"""
         # Bad BRDF
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(None, None, do_brdf='potato')
 
         # Bad masking
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(None, None, mask_bad='tomato')
 
         # Bad deletion
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(None, None, delete_when_done='parsnip')
 
     def test_badbands(self):
         """Test errors are raised if bad band / angle combinations are used."""
         # Bad band names
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, band_names='potato')
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, band_names=[])
-        with self.assertRaises(KeyError):
+        with pytest.raises(KeyError):
             PyCoxMunk(self.scn_good, band_names=['VIS008'])
 
         # Bad angle names
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=1.0)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names={})
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names={'sza': 1.})
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names={'sza': 1., 'vza': 1., })
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names={'sza': 1., 'vza': 1., 'saa': 1., })
         # Missing dataset in Scene
-        with self.assertRaises(KeyError):
+        with pytest.raises(KeyError):
             PyCoxMunk(self.scn_missing, self.good_bnd_names, angle_names=self.good_angle_names)
 
         # Good angle names
-        PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names)
 
     def test_ocean_color_init(self):
         """Test that ocean color options are parsed correctly."""
-        # Bad ocean color dir
-        with self.assertRaises(ValueError):
+        # Bad ocean color dirf
+        with pytest.raises(ValueError):
             PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names, oc_dir=1.0)
 
         # No ocean color dir
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names, oc_dir=None)
-        self.assertFalse(pcm.use_occci)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names, oc_dir=None)
+        assert not pcm.use_occci
 
         # Good ocean color dir
         ocdir = '/media/test_oc_dir/'
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names, oc_dir=ocdir)
-        self.assertTrue(pcm.use_occci)
-        self.assertEqual(pcm.oc_dir, ocdir)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names=self.good_angle_names, oc_dir=ocdir)
+        assert pcm.use_occci
+        assert pcm.oc_dir == ocdir
 
     def test_calcangles(self):
         """Check that angle calculation is initialised correctly."""
         mocker = mock.MagicMock()
         mocker_lalo = mock.MagicMock()
-        mocker_lalo.attrs['area'].get_lonlats_dask = self._get_lonlats
+        mocker_lalo.attrs['area'].get_lonlats = self._get_lonlats
         tmp_dict = {'VIS006': mocker_lalo,
                     'solar_zenith_angle': np.array([10, 10]),
                     'satellite_zenith_angle': np.array([10, 10]),
                     'solar_azimuth_angle': np.array([10, 10]),
                     'satellite_azimuth_angle': np.array([10, 10])}
         mocker.return_value = tmp_dict
         with mock.patch('pycoxmunk.CM_Main.cm_calcangles', mocker):
-            PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names='calc')
+            # Test a warning is raised, as we're passing some wind speeds of zero.
+            with pytest.warns(RuntimeWarning):
+                PyCoxMunk(self.scn_good, self.good_bnd_names, angle_names='calc')
             mocker.assert_called()
 
     def test_misc(self):
         """Misc tests for creation of the CM class."""
         # Bad Scene
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             PyCoxMunk(None, None)
 
     def test_wind_setup(self):
         """Test that winds are set up correctly."""
         mocker = mock.MagicMock()
         mocker.return_value = True
         with mock.patch('pycoxmunk.CM_Main.CMSharedWind', mocker):
-            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names)
+            with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+                pcm = PyCoxMunk(self.scn_good, self.good_bnd_names)
             pcm.setup_wind(13.4, -12.3)
-            self.assertTrue(pcm.shared_wind)
+            assert pcm.shared_wind
 
     def _make_mocked_cm_refl(self):
         cmr_mocker = mock.MagicMock()
 
         self.tmp_cmr_array = np.random.uniform(0, 10, (10, 10))
         self.tmp_cmr_array[0, 0] = -10.
 
@@ -184,108 +204,112 @@
         cmr_mocker.rhogl = True
         cmr_mocker.rhowc = True
 
         return cmr_mocker
 
     def test_pixmask(self):
         """Test that pixmask is correctly initialised in the class."""
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names)
-        self.assertTrue(pcm.pixmask is None)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names)
+        assert pcm.pixmask is None
         pcm.setup_pixmask(np.array([0, 0, 1]), np.array([2., 0, 0]), np.array([0., 0, 0]), np.array([1., 0, 1.]))
         np.testing.assert_allclose(pcm.pixmask.mask, np.array([1, 0, 1]))
 
     @mock.patch('pycoxmunk.CM_Main.calc_coxmunk_wrapper')
     def test_retr_cm(self, mock_cmr_func):
         """Tests for the main routine that retrieves reflectance."""
 
         cm_band_name = f'cox_munk_refl_{self.good_bnd_names[0]}'
         cm_rho0v_name = f'cox_munk_rho0v_{self.good_bnd_names[0]}'
 
         # This section tests that cox_munk reflectance is computed, but not BRDF
         # Recreate scene in case previous tests have messed with it.
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False)
         pcm.shared_wind = ['testval']
         pcm.retr_coxmunk_refl()
         np.testing.assert_allclose(pcm.scn[cm_band_name].data, self.tmp_cmr_array)
-        self.assertFalse(cm_rho0v_name in pcm.scn)
-        with self.assertRaises(AttributeError):
+        assert cm_rho0v_name not in pcm.scn
+        with pytest.raises(AttributeError):
             pcm.cm_refl.rhoul
 
         # Now we test for case when we also want the BRDF
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=True)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=True)
         pcm.retr_coxmunk_refl()
         np.testing.assert_allclose(pcm.scn[cm_band_name].data, self.tmp_cmr_array)
-        self.assertTrue(cm_rho0v_name in pcm.scn)
+        assert cm_rho0v_name in pcm.scn
         np.testing.assert_allclose(pcm.scn[cm_rho0v_name].data, self.tmp_cmr_array * 4)
 
         # Finally, test case where we mask bad values
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=True, do_brdf=True)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=True, do_brdf=True)
         pcm.retr_coxmunk_refl()
         new_arr = self.tmp_cmr_array.copy()
         new_arr[0, 0] = np.nan
         np.testing.assert_allclose(pcm.scn[cm_band_name].data, new_arr)
-        self.assertTrue(cm_rho0v_name in pcm.scn)
+        assert cm_rho0v_name in pcm.scn
         np.testing.assert_allclose(pcm.scn[cm_rho0v_name].data, new_arr * 4)
 
         # Now set up secondary pixmask class
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
         cmask = np.zeros((10, 10))
         cmask[5, 5] = 1
 
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=True, do_brdf=True)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=True, do_brdf=True)
         pcm.setup_pixmask(cloud_mask=cmask)
         pcm.retr_coxmunk_refl()
         new_arr = self.tmp_cmr_array.copy()
         new_arr[0, 0] = np.nan
         new_arr[5, 5] = np.nan
         np.testing.assert_allclose(pcm.scn[cm_band_name].data, new_arr)
 
-
     @mock.patch('pycoxmunk.CM_Main.calc_coxmunk_wrapper')
     def test_deleter(self, mock_cmr_func):
         """Test that deletions are done correctly."""
 
-        cm_band_name = f'cox_munk_refl_{self.good_bnd_names[0]}'
-        cm_rho0v_name = f'cox_munk_rho0v_{self.good_bnd_names[0]}'
-
         tmp_arr = np.array([1, 4., 64])
 
         # Test for case where we don't delete intermediate data
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False, delete_when_done=False)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False, delete_when_done=False)
         pcm.shared_wind = tmp_arr
         pcm.geometry = 'geotest'
         pcm.cm_refl.rhogl = True
         pcm._run_delete()
-        self.assertEqual(pcm.geometry, 'geotest')
-        self.assertEqual(pcm.cm_refl.rhogl, True)
+        assert pcm.geometry == 'geotest'
+        assert pcm.cm_refl.rhogl
         np.testing.assert_allclose(pcm.shared_wind, tmp_arr)
 
         # Test for case where we delete intermediate data
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False, delete_when_done=True)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False, delete_when_done=True)
         pcm.shared_wind = tmp_arr
         pcm.geometry = 'geotest'
         pcm._run_delete()
-        self.assertFalse(hasattr(pcm, 'geometry'))
-        self.assertFalse(hasattr(pcm.cm_refl, 'rhogl'))
-        self.assertFalse(hasattr(pcm, 'shared_wind'))
+        assert not hasattr(pcm, 'geometry')
+        assert not hasattr(pcm.cm_refl, 'rhogl')
+        assert not hasattr(pcm, 'shared_wind')
 
         # Test for case where we delete intermediate data with some missing
         self.scn_good = self.create_test_scene(self.good_bnd_names, self.good_angle_names)
         mock_cmr_func.return_value = self._make_mocked_cm_refl()
-        pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False, delete_when_done=True)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            pcm = PyCoxMunk(self.scn_good, self.good_bnd_names, mask_bad=False, do_brdf=False, delete_when_done=True)
         del pcm.shared_wind
         del pcm.geometry
         del pcm.cm_refl.rhogl
         del pcm.cm_refl.rhoul
         del pcm.cm_refl.rhowc
         pcm._run_delete()
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/Tests/test_PixMask.py` & `pycoxmunk-1.1.0/pycoxmunk/Tests/test_PixMask.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
 """Test the pixel masking module."""
 
-import unittest
 import numpy as np
 from pycoxmunk.CM_PixMask import CMPixMask
 
 
-class TestCMPixMask(unittest.TestCase):
+class TestCMPixMask:
     """Test the various pixel masking methods."""
-    def setUp(self):
+    def setup_method(self):
         """Set up the initial data."""
         self.zens = np.array([0., 0.01, 12., 15, 45.35, 79.99, 84.23, 91.1, 112.12, -10.])
         self.cloud_mask = np.array([0, 1, 1, 0, 0, 0, 0, 1, 1, 1])
         self.sol_mask = np.array([1, 1, 1, 1, 0, 0, 1, 0, 0, 1])
         self.sat_mask = np.array([0, 0, 1, 0, 1, 0, 0, 0, 0, 1])
         self.land_mask = np.array([1, 0, 0, 0, 1, 1, 1, 1, 1, 0])
 
@@ -37,15 +35,15 @@
         self.test_zenmask = np.array([0, 1, 1, 0, 0, 0, 1, 1, 1, 1])
         self.test_zenmask2 = np.array([0, 0, 0, 0, 0, 1, 1, 1, 1, 0])
 
     def test_init(self):
         """Test the masks are combined correctly."""
         # No masks
         main_mask = CMPixMask()
-        self.assertEqual(main_mask.mask, None)
+        assert main_mask.mask is None
 
         main_mask = CMPixMask(cloud_mask=self.cloud_mask)
         np.testing.assert_allclose(main_mask.mask, self.cloud_mask)
 
         main_mask = CMPixMask(cloud_mask=self.cloud_mask, sol_zen_mask=self.sol_mask)
         np.testing.assert_allclose(main_mask.mask, self.test_mask)
 
@@ -54,10 +52,7 @@
         main_mask = CMPixMask(cloud_mask=self.cloud_mask)
         main_mask.cut_high_zen(self.zens)
         np.testing.assert_allclose(main_mask.mask, self.test_zenmask)
 
         main_mask = CMPixMask()
         main_mask.cut_high_zen(self.zens, threshold=70)
         np.testing.assert_allclose(main_mask.mask, self.test_zenmask2)
-
-
-
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/Tests/test_SceneGeom.py` & `pycoxmunk-1.1.0/pycoxmunk/Tests/test_SceneGeom.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
 """Test the scene geometry module."""
 
 from pycoxmunk.CM_SceneGeom import CMSceneGeom as Cm_sg
 from pycoxmunk.CM_SceneGeom import cm_calcangles
 from unittest import mock
 import numpy as np
 import unittest
+import pytest
 
 
 class TestSceneGeom(unittest.TestCase):
     def setUp(self):
         """Set up some common variables for the tests."""
         self.sza = np.array([58.655, 167.412, 3.173, 63.215])
         self.vza = np.array([57.733, 21.248, 57.777, 99.768])
@@ -50,16 +50,17 @@
             calc_func.assert_not_called()
 
         # Check returned values are correct in case of single values
         geom = Cm_sg(1., 50., 1., 30., 1., 1.)
         self.assertAlmostEqual(geom.raa, 20.)
 
         # And likewise for arrays
-        geom = Cm_sg(self.sza, self.saa, self.vza,
-                     self.vaa, self.lats, self.lons)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            geom = Cm_sg(self.sza, self.saa, self.vza,
+                         self.vaa, self.lats, self.lons)
         np.testing.assert_allclose(geom.raa, self.raa)
 
     @mock.patch('satpy.modifiers.angles._get_sensor_angles')
     @mock.patch('satpy.modifiers.angles._get_sun_angles')
     def test_calcangles(self, get_sun, get_sat):
         """Test user-requested angle calculation."""
         from satpy import Scene
@@ -73,113 +74,127 @@
         retr = cm_calcangles(test_scn, 'VIS006')
         np.testing.assert_allclose(retr['solar_zenith_angle'].data, self.sza)
         np.testing.assert_allclose(retr['solar_azimuth_angle'].data, self.saa)
         np.testing.assert_allclose(retr['satellite_zenith_angle'].data, self.vza)
         np.testing.assert_allclose(retr['satellite_azimuth_angle'].data, self.vaa)
 
         # Check what happens if bad refband is passed
-        with self.assertRaises(KeyError):
+        with pytest.raises(KeyError):
             cm_calcangles(test_scn, 'VIS008')
 
         # Check if we pass bad data
-        with self.assertRaises(KeyError):
+        with pytest.raises(KeyError):
             test_scn['VIS006'] = xr.DataArray(np.array([[5., 4.], [4., 5.]]))
             cm_calcangles(test_scn, 'VIS008')
 
         # Check error is raised if angles can't be computed
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             get_sun.side_effect = ValueError("Bad data")
             cm_calcangles(test_scn, 'VIS006')
 
-
     def test_shapechecker(self):
         """Tests for the shape checker that ensures arrays are same size."""
         # Default case
-        Cm_sg(self.sza, self.saa, self.vza,
-              self.vaa, self.lats, self.lons)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            Cm_sg(self.sza, self.saa, self.vza,
+                  self.vaa, self.lats, self.lons)
 
         # Mismatched arrays
-        with self.assertRaises(AssertionError):
-            Cm_sg(self.sza, self.saa, self.vza,
-                  self.vaa, np.array([1., 2.]), self.lons)
+        with pytest.raises(AssertionError):
+            with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+                Cm_sg(self.sza, self.saa, self.vza,
+                      self.vaa, np.array([1., 2.]), self.lons)
 
         # One array, rest scalar
         with mock.patch('pycoxmunk.CM_SceneGeom.CMSceneGeom.calc_relazi') as calc_func:
             calc_func.return_value = 1.
-            retr = Cm_sg(self.sza, 5., 3., -10., 15., -21.)
+            with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+                retr = Cm_sg(self.sza, 5., 3., -10., 15., -21.)
             self.assertEqual(len(retr.sza), 4)
             self.assertEqual(retr.saa, 5.)
 
     def test_bounds_checker(self):
         """Ensure that bounds checks catch bad input data"""
         # SZA
         test_cmsg = Cm_sg(0., 0., 0., 0., 0., 0.)
-        Cm_sg(test_cmsg.zenith_min - 5, 1., 1., 1., 1., 1.)
-        with self.assertRaises(ValueError):
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            Cm_sg(test_cmsg.zenith_min - 5, 1., 1., 1., 1., 1.)
+        with pytest.raises(ValueError):
             Cm_sg(test_cmsg.zenith_min - 5, 1., 1., 1., 1., 1., fix_angs=False)
 
-        Cm_sg(test_cmsg.zenith_max + 100., 1., 1., 1., 1., 1.)
-        with self.assertRaises(ValueError):
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            Cm_sg(test_cmsg.zenith_max + 100., 1., 1., 1., 1., 1.)
+        with pytest.raises(ValueError):
             Cm_sg(test_cmsg.zenith_max + 100., 1., 1., 1., 1., 1., fix_angs=False)
         Cm_sg(test_cmsg.zenith_max - 10., 1., 1., 1., 1., 1.)
 
         # SAA
-        Cm_sg(1., test_cmsg.azimuth_min - 20., 1., 1., 1., 1.)
-        with self.assertRaises(ValueError):
+        with pytest.warns(UserWarning, match="Some solar azimuth values out of range. Scaling."):
+            Cm_sg(1., test_cmsg.azimuth_min - 20., 1., 1., 1., 1.)
+        with pytest.raises(ValueError):
             Cm_sg(1., test_cmsg.azimuth_min - 20., 1., 1., 1., 1., fix_angs=False)
         Cm_sg(1., test_cmsg.azimuth_min + 20., 1., 1., 1., 1.)
 
-        Cm_sg(1., test_cmsg.azimuth_max + 20., 1., 1., 1., 1.)
-        with self.assertRaises(ValueError):
+        with pytest.warns(UserWarning, match="Some solar azimuth values out of range. Scaling."):
+            Cm_sg(1., test_cmsg.azimuth_max + 20., 1., 1., 1., 1.)
+        with pytest.raises(ValueError):
             Cm_sg(1., test_cmsg.azimuth_max + 20., 1., 1., 1., 1., fix_angs=False)
         Cm_sg(1., test_cmsg.azimuth_max - 20., 1., 1., 1., 1.)
 
         # VZA
-        Cm_sg(1., 1., test_cmsg.zenith_min - 15., 1., 1., 1.)
-        with self.assertRaises(ValueError):
-            Cm_sg(1., 1., test_cmsg.zenith_min - 15., 1., 1., 1., fix_angs=False)
+        with pytest.warns(UserWarning, match="Some satellite zenith values out of range. Clipping."):
+            Cm_sg(1., 1., test_cmsg.zenith_min - 15., 1., 1., 1.)
+        with pytest.raises(ValueError):
+            with pytest.warns(UserWarning, match="Some satellite zenith values out of range. Clipping."):
+                Cm_sg(1., 1., test_cmsg.zenith_min - 15., 1., 1., 1., fix_angs=False)
         Cm_sg(1., 1., test_cmsg.zenith_min + 10., 1., 1., 1.)
 
-        Cm_sg(1., 1., test_cmsg.zenith_max + 15., 1., 1., 1.)
-        with self.assertRaises(ValueError):
-            Cm_sg(1., 1., test_cmsg.zenith_max + 15., 1., 1., 1., fix_angs=False)
+        with pytest.warns(UserWarning, match="Some satellite zenith values out of range. Clipping."):
+            Cm_sg(1., 1., test_cmsg.zenith_max + 15., 1., 1., 1.)
+        with pytest.raises(ValueError):
+            with pytest.warns(UserWarning, match="Some satellite zenith values out of range. Clipping."):
+                Cm_sg(1., 1., test_cmsg.zenith_max + 15., 1., 1., 1., fix_angs=False)
         Cm_sg(1., 1., test_cmsg.zenith_max - 10., 1., 1., 1.)
 
         # VAA
-        Cm_sg(1., 1., 1., test_cmsg.azimuth_min - 25., 1., 1.)
-        with self.assertRaises(ValueError):
-            Cm_sg(1., 1., 1., test_cmsg.azimuth_min - 25., 1., 1., fix_angs=False)
+        with pytest.warns(UserWarning, match="Some satellite azimuth values out of range. Scaling."):
+            Cm_sg(1., 1., 1., test_cmsg.azimuth_min - 25., 1., 1.)
+        with pytest.raises(ValueError):
+            with pytest.warns(UserWarning, match="Some satellite azimuth values out of range. Scaling."):
+                Cm_sg(1., 1., 1., test_cmsg.azimuth_min - 25., 1., 1., fix_angs=False)
         Cm_sg(1., 1., 1., test_cmsg.azimuth_min + 1., 1., 1.)
 
-        Cm_sg(1., 1., 1., test_cmsg.azimuth_max + 50., 1., 1.)
-        with self.assertRaises(ValueError):
-            Cm_sg(1., 1., 1., test_cmsg.azimuth_max + 50., 1., 1., fix_angs=False)
+        with pytest.warns(UserWarning, match="Some satellite azimuth values out of range. Scaling."):
+            Cm_sg(1., 1., 1., test_cmsg.azimuth_max + 50., 1., 1.)
+        with pytest.raises(ValueError):
+            with pytest.warns(UserWarning, match="Some satellite azimuth values out of range. Scaling."):
+                Cm_sg(1., 1., 1., test_cmsg.azimuth_max + 50., 1., 1., fix_angs=False)
         Cm_sg(1., 1., 1., test_cmsg.azimuth_max - 1., 1., 1.)
 
         # Lats
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             Cm_sg(1., 1., 1., 1., test_cmsg.lat_min - 25., 1.)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             Cm_sg(1., 1., 1., 1., test_cmsg.lat_max + 25., 1.)
         Cm_sg(1., 1., 1., 1., test_cmsg.lat_max - 15., 1.)
 
         # Lons
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             Cm_sg(1., 1., 1., 1., 1., test_cmsg.lon_min - 0.01)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             Cm_sg(1., 1., 1., 1., 1., test_cmsg.lon_max + 10.)
         Cm_sg(1., 1., 1., 1., 1., test_cmsg.lon_min + 0.01)
 
         # RAA
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             Cm_sg(1., 1., 1., 1., 1., 1., check_raa=True, raa=test_cmsg.relazi_min - 10.)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             Cm_sg(1., 1., 1., 1., 1., 1., raa=test_cmsg.relazi_max + 11., fix_angs=False, check_raa=True)
         Cm_sg(1., 1., 1., 1., 1., 1., raa=test_cmsg.relazi_min + 10., fix_angs=False, check_raa=True)
 
         # Also do one test for the case where we pass arrays
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             tmp_arr = np.array([1., 1.])
             Cm_sg(np.array([test_cmsg.zenith_min - 5., 1.]), tmp_arr, tmp_arr,
                   tmp_arr, tmp_arr, tmp_arr, fix_angs=False)
         Cm_sg(tmp_arr, tmp_arr, tmp_arr,
               tmp_arr, tmp_arr, tmp_arr)
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/Tests/test_SharedWind.py` & `pycoxmunk-1.1.0/pycoxmunk/Tests/test_SharedWind.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
 """Test the scene geometry module."""
 
 from pycoxmunk.CM_Shared_Wind import CMSharedWind
 from pycoxmunk.CM_SceneGeom import CMSceneGeom
 import numpy as np
-import unittest
+import pytest
 
 
-class TestSharedWind(unittest.TestCase):
-    def setUp(self):
+class TestSharedWind:
+    def setup_method(self):
         """Set up some common variables for the tests."""
         self.u10 = np.array([15., -4., -1, 10.7])
         self.v10 = np.array([8.1, 4.0, 11.9, -8.1])
 
         self.ws = np.array([17.04728717, 5.65685425, 11.94194289, 13.42013413])
         self.wd = np.array([2.38240853, 4.74502664, 5.37000261, 4.60018284])
         self.wcfrac = np.array([0.06388454, 0.00131533, 0.01825043, 0.02752158])
@@ -42,21 +41,21 @@
         self.vza = np.array([57.733, 21.248, 87.777, 99.768])
         self.saa = np.array([285.129, 133.130, 57.125, 223.555])
         self.vaa = np.array([38.505, 185.793, 133.017, 341.330])
         self.raa = np.array([113.376, 52.663, 75.892, 117.775])
         self.lats = np.array([-5.247, -58.473, 17.666, 48.237])
         self.lons = np.array([-116.184, 73.047, 120.744, -121.522])
 
-        self.scene_geom = CMSceneGeom(self.sza, self.saa, self.vza, self.vaa, self.lats, self.lons, raa=self.raa)
+        with pytest.warns(UserWarning, match="Some solar zenith values out of range. Clipping."):
+            self.scene_geom = CMSceneGeom(self.sza, self.saa, self.vza, self.vaa, self.lats, self.lons, raa=self.raa)
 
     def test_sharedwind(self):
         """Test the calculation of relative azimuth angles."""
         sh_wind = CMSharedWind(self.scene_geom, self.u10, self.v10)
         np.testing.assert_allclose(sh_wind.ws, self.ws, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.wd, self.wd, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.wcfrac, self.wcfrac, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.ergodic, self.ergodic, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.cosomega, self.cosomega, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.cosbeta, self.cosbeta, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.w, self.w, rtol=1e-5)
         np.testing.assert_allclose(sh_wind.p, self.p, rtol=1e-5)
-
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/Tests/test_Utils.py` & `pycoxmunk-1.1.0/pycoxmunk/Tests/test_Utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,56 +2,54 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
 """Test the scene geometry module."""
 from pycoxmunk import CM_Utils
 import xarray as xrd
-from unittest import mock
 import numpy as np
-import unittest
+import pytest
 
 
-class TestUtils(unittest.TestCase):
+class TestUtils:
     def test_typechecker(self):
         """Checks for array/value types."""
         CM_Utils.check_type(1., 'test')
         CM_Utils.check_type(np.array([1.]), 'test')
         CM_Utils.check_type(np.array([1]), 'test')
         CM_Utils.check_type(xrd.DataArray(np.array([1])), 'test')
-        with self.assertRaises(TypeError):
+        with pytest.raises(TypeError):
             CM_Utils.check_type([1.], 'test')
-        with self.assertRaises(TypeError):
+        with pytest.raises(TypeError):
             CM_Utils.check_type(1, 'test')
 
     def test_check_and_reshape(self):
         """Test the array resizer"""
 
         test_arr = np.random.uniform(0, 1, 10)
         out_arr = CM_Utils.check_and_reshape(test_arr, (10,))
 
-        self.assertEqual(out_arr.shape, test_arr.shape)
-        with self.assertRaises(ValueError):
+        assert out_arr.shape == test_arr.shape
+        with pytest.raises(ValueError):
             CM_Utils.check_and_reshape(test_arr, 100)
 
         test_arr = np.random.uniform(0, 1, 1)
         out_arr = CM_Utils.check_and_reshape(test_arr, 10)
-        self.assertEqual(out_arr.shape, (10,))
+        assert out_arr.shape == (10,)
 
     def test_gauss_leg(self):
         """Test the Gauss-Legendre calculations."""
 
         w, x = CM_Utils.gauss_leg_quadx(5, 0, 10)
         expected = np.array([1.18463443, 2.39314335, 2.84444444, 2.39314335, 1.18463443])
         np.testing.assert_almost_equal(x, expected)
@@ -69,9 +67,9 @@
         np.testing.assert_almost_equal(x, expected)
 
         w, x = CM_Utils.gauss_leg_quadx(12, 1, 100)
         expected = np.array([2.33517915, 5.29349664, 7.92387726, 10.05678762, 11.55788056, 12.33277877,
                              12.33277877, 11.55788056, 10.05678762, 7.92387726, 5.29349664, 2.33517915])
         np.testing.assert_almost_equal(x, expected)
 
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             CM_Utils.gauss_leg_quadx(0, -10, 10)
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk/__init__.py` & `pycoxmunk-1.1.0/pycoxmunk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2022 Simon R Proud
 #
 # This file is part of PyCoxMunk.
 #
 # PyCoxMunk is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
+# Foundation, version 3.
 #
 # PyCoxMunk is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PyCoxMunk.  If not, see <http://www.gnu.org/licenses/>.
 
 
 """For instructions on using pycoxmunk please see the documentation under the pycoxmunk.PyCoxMunk class."""
 
-from pycoxmunk.CM_Main import PyCoxMunk
+from pycoxmunk.CM_Main import PyCoxMunk  # noqa
```

### Comparing `pycoxmunk-1.0.0/pycoxmunk.egg-info/SOURCES.txt` & `pycoxmunk-1.1.0/pycoxmunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycoxmunk-1.0.0/pyproject.toml` & `pycoxmunk-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pycoxmunk"
-version = "1.0.0"
+version = "1.1.0"
 description = "An algorithm to compute sea surface reflectance using the Cox-Munk approach."
 readme = "README.md"
 authors = [{ name = "Simon R Proud", email = "simon.proud@stfc.ac.uk" }]
-license = { file = "LICENSE" }
+license = { text = "GPLv3" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["satellite", "oceanography", "remote-sensing", "earth-observation", "reflectance"]
 dependencies = [
```

### Comparing `pycoxmunk-1.0.0/setup.cfg` & `pycoxmunk-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 6f78 6d75 6e6b 0d0a 7665   = pycoxmunk..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 300d 0a61  rsion = 1.0.0..a
+00000020: 7273 696f 6e20 3d20 312e 312e 300d 0a61  rsion = 1.1.0..a
 00000030: 7574 686f 7220 3d20 5369 6d6f 6e20 5220  uthor = Simon R 
 00000040: 5072 6f75 640d 0a61 7574 686f 725f 656d  Proud..author_em
 00000050: 6169 6c20 3d20 7369 6d6f 6e2e 7072 6f75  ail = simon.prou
 00000060: 6440 7374 6663 2e61 632e 756b 0d0a 6465  d@stfc.ac.uk..de
 00000070: 7363 7269 7074 696f 6e20 3d20 416e 2061  scription = An a
 00000080: 6c67 6f72 6974 686d 2074 6f20 636f 6d70  lgorithm to comp
 00000090: 7574 6520 7365 6120 7375 7266 6163 6520  ute sea surface 
@@ -24,17 +24,17 @@
 00000170: 3a2f 2f67 6974 6875 622e 636f 6d2f 7369  ://github.com/si
 00000180: 6d6f 6e72 7038 342f 5079 436f 784d 756e  monrp84/PyCoxMun
 00000190: 6b2f 6973 7375 6573 0d0a 636c 6173 7369  k/issues..classi
 000001a0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
 000001b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 000001c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
 000001d0: 094c 4943 454e 5345 203a 3a20 4f53 4920  .LICENSE :: OSI 
-000001e0: 4150 5052 4f56 4544 203a 3a20 474e 5520  APPROVED :: GNU 
-000001f0: 4745 4e45 5241 4c20 5055 424c 4943 204c  GENERAL PUBLIC L
-00000200: 4943 454e 5345 2056 3320 2847 504c 5633  ICENSE V3 (GPLV3
+000001e0: 4170 7072 6f76 6564 203a 3a20 474e 5520  Approved :: GNU 
+000001f0: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
+00000200: 6963 656e 7365 2076 3320 2847 504c 7633  icense v3 (GPLv3
 00000210: 290d 0a09 4f70 6572 6174 696e 6720 5379  )...Operating Sy
 00000220: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
 00000230: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
 00000240: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
 00000250: 203d 200d 0a09 3d2e 0d0a 7061 636b 6167   = ...=...packag
 00000260: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
 00000270: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
```

