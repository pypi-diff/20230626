# Comparing `tmp/rainbow-connection-0.0.6.tar.gz` & `tmp/rainbow-connection-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rainbow-connection-0.0.6.tar", last modified: Fri Nov 13 03:53:14 2020, max compression
+gzip compressed data, was "dist/rainbow-connection-0.0.7.tar", last modified: Mon May 10 15:21:50 2021, max compression
```

## Comparing `rainbow-connection-0.0.6.tar` & `rainbow-connection-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,60 @@
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.348290 rainbow-connection-0.0.6/
--rw-r--r--   0 bt         (501) staff       (20)      114 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/MANIFEST.in
--rw-r--r--   0 bt         (501) staff       (20)      608 2020-11-13 03:53:14.347876 rainbow-connection-0.0.6/PKG-INFO
--rw-r--r--   0 bt         (501) staff       (20)     2024 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/README.md
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.332585 rainbow-connection-0.0.6/rainbow_connection.egg-info/
--rw-r--r--   0 bt         (501) staff       (20)      608 2020-11-13 03:53:14.000000 rainbow-connection-0.0.6/rainbow_connection.egg-info/PKG-INFO
--rw-r--r--   0 bt         (501) staff       (20)     1585 2020-11-13 03:53:14.000000 rainbow-connection-0.0.6/rainbow_connection.egg-info/SOURCES.txt
--rw-r--r--   0 bt         (501) staff       (20)        1 2020-11-13 03:53:14.000000 rainbow-connection-0.0.6/rainbow_connection.egg-info/dependency_links.txt
--rw-r--r--   0 bt         (501) staff       (20)        1 2020-11-12 02:09:56.000000 rainbow-connection-0.0.6/rainbow_connection.egg-info/not-zip-safe
--rw-r--r--   0 bt         (501) staff       (20)       85 2020-11-13 03:53:14.000000 rainbow-connection-0.0.6/rainbow_connection.egg-info/requires.txt
--rw-r--r--   0 bt         (501) staff       (20)       18 2020-11-13 03:53:14.000000 rainbow-connection-0.0.6/rainbow_connection.egg-info/top_level.txt
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.335228 rainbow-connection-0.0.6/rainbowconnection/
--rw-r--r--   0 bt         (501) staff       (20)      165 2020-11-13 03:50:33.000000 rainbow-connection-0.0.6/rainbowconnection/__init__.py
--rw-r--r--   0 bt         (501) staff       (20)      789 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/animatetools.py
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.337820 rainbow-connection-0.0.6/rainbowconnection/atmospheres/
--rw-r--r--   0 bt         (501) staff       (20)      167 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/__init__.py
--rw-r--r--   0 bt         (501) staff       (20)    11931 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/atmosphere.py
--rw-r--r--   0 bt         (501) staff       (20)     1403 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/earth.py
--rw-r--r--   0 bt         (501) staff       (20)     2281 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/exoplanet.py
--rw-r--r--   0 bt         (501) staff       (20)     1556 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/hotjupiter.py
--rw-r--r--   0 bt         (501) staff       (20)     1886 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/noatmosphere.py
--rw-r--r--   0 bt         (501) staff       (20)     3812 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/sky.py
--rw-r--r--   0 bt         (501) staff       (20)    19888 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/atmospheres/sunset.py
--rw-r--r--   0 bt         (501) staff       (20)     5472 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/colortools.py
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.338652 rainbow-connection-0.0.6/rainbowconnection/data/
--rw-r--r--   0 bt         (501) staff       (20)    68262 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/data/earthtransmission.txt
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.342157 rainbow-connection-0.0.6/rainbowconnection/data/fortney/
--rw-r--r--   0 bt         (501) staff       (20)      153 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/data/fortney/README.txt
--rwxr-xr-x   0 bt         (501) staff       (20)  1380037 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/data/fortney/lambda_1500K_g10_noTiOVO.dat
--rwxr-xr-x   0 bt         (501) staff       (20)  1380037 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/data/fortney/lambda_1500K_g10_wTiOVO.dat
--rw-r--r--   0 bt         (501) staff       (20)    14012 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/data/solarspectrum.txt
--rw-r--r--   0 bt         (501) staff       (20)      599 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/imports.py
--rw-r--r--   0 bt         (501) staff       (20)     1241 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/plottingtools.py
--rw-r--r--   0 bt         (501) staff       (20)    10342 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/resampletools.py
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.346107 rainbow-connection-0.0.6/rainbowconnection/sources/
--rw-r--r--   0 bt         (501) staff       (20)    20983 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/sources/Spectrum.py
--rw-r--r--   0 bt         (501) staff       (20)     3415 2020-11-12 04:32:05.000000 rainbow-connection-0.0.6/rainbowconnection/sources/Thermal.py
--rw-r--r--   0 bt         (501) staff       (20)      220 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/__init__.py
--rw-r--r--   0 bt         (501) staff       (20)      226 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/blank.py
--rw-r--r--   0 bt         (501) staff       (20)     2177 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/sources/lightbulbs.py
-drwxr-xr-x   0 bt         (501) staff       (20)        0 2020-11-13 03:53:14.347511 rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/
--rw-r--r--   0 bt         (501) staff       (20)       43 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/__init__.py
--rw-r--r--   0 bt         (501) staff       (20)     8937 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/library.py
--rw-r--r--   0 bt         (501) staff       (20)     1648 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/star.py
--rw-r--r--   0 bt         (501) staff       (20)      330 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/utils.py
--rw-r--r--   0 bt         (501) staff       (20)     1431 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/rainbowconnection/sources/sun.py
--rw-r--r--   0 bt         (501) staff       (20)      998 2020-10-14 13:04:52.000000 rainbow-connection-0.0.6/rainbowconnection/units.py
--rw-r--r--   0 bt         (501) staff       (20)       22 2020-11-13 03:50:38.000000 rainbow-connection-0.0.6/rainbowconnection/version.py
--rw-r--r--   0 bt         (501) staff       (20)       38 2020-11-13 03:53:14.348439 rainbow-connection-0.0.6/setup.cfg
--rw-r--r--   0 bt         (501) staff       (20)     3648 2020-11-12 04:28:01.000000 rainbow-connection-0.0.6/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.961203 rainbow-connection-0.0.7/
+-rw-r--r--   0 zach       (502) staff       (20)     1260 2021-01-22 20:52:04.000000 rainbow-connection-0.0.7/.gitignore
+-rw-r--r--   0 zach       (502) staff       (20)     1088 2021-01-22 20:58:26.000000 rainbow-connection-0.0.7/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)      114 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/MANIFEST.in
+-rw-r--r--   0 zach       (502) staff       (20)      608 2021-05-10 15:21:50.960976 rainbow-connection-0.0.7/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2024 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/README.md
+-rw-r--r--   0 zach       (502) staff       (20)    53734 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/earth-sunset.png
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.944918 rainbow-connection-0.0.7/rainbow_connection.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)      608 2021-05-10 15:21:50.000000 rainbow-connection-0.0.7/rainbow_connection.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     1681 2021-05-10 15:21:50.000000 rainbow-connection-0.0.7/rainbow_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2021-05-10 15:21:50.000000 rainbow-connection-0.0.7/rainbow_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2021-01-22 15:54:09.000000 rainbow-connection-0.0.7/rainbow_connection.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)       85 2021-05-10 15:21:50.000000 rainbow-connection-0.0.7/rainbow_connection.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       18 2021-05-10 15:21:50.000000 rainbow-connection-0.0.7/rainbow_connection.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.948348 rainbow-connection-0.0.7/rainbowconnection/
+-rw-r--r--   0 zach       (502) staff       (20)      199 2021-01-25 04:49:58.000000 rainbow-connection-0.0.7/rainbowconnection/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      933 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/animatetools.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.951624 rainbow-connection-0.0.7/rainbowconnection/atmospheres/
+-rw-r--r--   0 zach       (502) staff       (20)      167 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)    12106 2021-01-25 04:08:34.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/atmosphere.py
+-rw-r--r--   0 zach       (502) staff       (20)     1430 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/earth.py
+-rw-r--r--   0 zach       (502) staff       (20)     2280 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/exoplanet.py
+-rw-r--r--   0 zach       (502) staff       (20)     1582 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/hotjupiter.py
+-rw-r--r--   0 zach       (502) staff       (20)     1891 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/noatmosphere.py
+-rw-r--r--   0 zach       (502) staff       (20)     3882 2021-01-25 04:08:34.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/sky.py
+-rw-r--r--   0 zach       (502) staff       (20)    19943 2021-01-25 04:08:34.000000 rainbow-connection-0.0.7/rainbowconnection/atmospheres/sunset.py
+-rw-r--r--   0 zach       (502) staff       (20)     7775 2021-01-25 04:25:00.000000 rainbow-connection-0.0.7/rainbowconnection/colortools.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.952513 rainbow-connection-0.0.7/rainbowconnection/data/
+-rw-r--r--   0 zach       (502) staff       (20)    68262 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/data/earthtransmission.txt
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.954507 rainbow-connection-0.0.7/rainbowconnection/data/fortney/
+-rw-r--r--   0 zach       (502) staff       (20)      153 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/data/fortney/README.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)  1380037 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/data/fortney/lambda_1500K_g10_noTiOVO.dat
+-rwxr-xr-x   0 zach       (502) staff       (20)  1380037 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/data/fortney/lambda_1500K_g10_wTiOVO.dat
+-rw-r--r--   0 zach       (502) staff       (20)    14012 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/data/solarspectrum.txt
+-rw-r--r--   0 zach       (502) staff       (20)      629 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/imports.py
+-rw-r--r--   0 zach       (502) staff       (20)     1195 2021-01-25 04:08:33.000000 rainbow-connection-0.0.7/rainbowconnection/plottingtools.py
+-rw-r--r--   0 zach       (502) staff       (20)    10434 2021-05-10 15:17:16.000000 rainbow-connection-0.0.7/rainbowconnection/resampletools.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.957491 rainbow-connection-0.0.7/rainbowconnection/sources/
+-rw-r--r--   0 zach       (502) staff       (20)      175 2021-01-27 06:01:44.000000 rainbow-connection-0.0.7/rainbowconnection/sources/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      226 2021-01-22 20:29:13.000000 rainbow-connection-0.0.7/rainbowconnection/sources/blank.py
+-rw-r--r--   0 zach       (502) staff       (20)     5021 2021-03-11 03:18:49.000000 rainbow-connection-0.0.7/rainbowconnection/sources/lightbulbs.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.958815 rainbow-connection-0.0.7/rainbowconnection/sources/phoenix/
+-rw-r--r--   0 zach       (502) staff       (20)       43 2021-01-22 15:39:06.000000 rainbow-connection-0.0.7/rainbowconnection/sources/phoenix/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)    11538 2021-05-10 15:16:33.000000 rainbow-connection-0.0.7/rainbowconnection/sources/phoenix/library.py
+-rw-r--r--   0 zach       (502) staff       (20)     1885 2021-05-10 15:15:08.000000 rainbow-connection-0.0.7/rainbowconnection/sources/phoenix/star.py
+-rw-r--r--   0 zach       (502) staff       (20)      331 2021-01-22 20:29:13.000000 rainbow-connection-0.0.7/rainbowconnection/sources/phoenix/utils.py
+-rw-r--r--   0 zach       (502) staff       (20)    23764 2021-05-10 15:17:16.000000 rainbow-connection-0.0.7/rainbowconnection/sources/spectrum.py
+-rw-r--r--   0 zach       (502) staff       (20)     1495 2021-01-25 04:08:34.000000 rainbow-connection-0.0.7/rainbowconnection/sources/sun.py
+-rw-r--r--   0 zach       (502) staff       (20)     3453 2021-01-25 04:08:34.000000 rainbow-connection-0.0.7/rainbowconnection/sources/thermal.py
+-rw-r--r--   0 zach       (502) staff       (20)      994 2021-01-22 20:29:13.000000 rainbow-connection-0.0.7/rainbowconnection/units.py
+-rw-r--r--   0 zach       (502) staff       (20)       22 2021-05-10 15:20:44.000000 rainbow-connection-0.0.7/rainbowconnection/version.py
+-rw-r--r--   0 zach       (502) staff       (20)       38 2021-05-10 15:21:50.961256 rainbow-connection-0.0.7/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     3648 2021-01-22 20:42:31.000000 rainbow-connection-0.0.7/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2021-05-10 15:21:50.960665 rainbow-connection-0.0.7/tests/
+-rw-r--r--   0 zach       (502) staff       (20)      241 2021-01-22 20:48:30.000000 rainbow-connection-0.0.7/tests/directory.py
+-rw-r--r--   0 zach       (502) staff       (20)      611 2021-01-22 20:50:27.000000 rainbow-connection-0.0.7/tests/test_atmospheres.py
+-rw-r--r--   0 zach       (502) staff       (20)      796 2021-01-22 20:50:27.000000 rainbow-connection-0.0.7/tests/test_lights.py
+-rw-r--r--   0 zach       (502) staff       (20)      587 2021-05-10 15:15:19.000000 rainbow-connection-0.0.7/tests/test_phoenix.py
+-rw-r--r--   0 zach       (502) staff       (20)     3771 2021-01-22 20:50:27.000000 rainbow-connection-0.0.7/tests/test_resampling.py
+-rw-r--r--   0 zach       (502) staff       (20)      673 2021-01-22 20:50:47.000000 rainbow-connection-0.0.7/tests/test_sunsets.py
```

### Comparing `rainbow-connection-0.0.6/PKG-INFO` & `rainbow-connection-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rainbow-connection
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pedagogical tools for light and color in astronomy.
 Home-page: https://github.com/zkbt/rainbow-connection
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Description: For detailed usage, please read the documentation at https://zkbt.github.io/rainbow-connection/.
 Platform: UNKNOWN
```

### Comparing `rainbow-connection-0.0.6/README.md` & `rainbow-connection-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rainbow-connection-0.0.6/rainbow_connection.egg-info/PKG-INFO` & `rainbow-connection-0.0.7/rainbow_connection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rainbow-connection
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pedagogical tools for light and color in astronomy.
 Home-page: https://github.com/zkbt/rainbow-connection
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Description: For detailed usage, please read the documentation at https://zkbt.github.io/rainbow-connection/.
 Platform: UNKNOWN
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/atmosphere.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/atmosphere.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from ..imports import *
 from ..units import determine_quantity
 from ..plottingtools import setup_axes_with_rainbow
 from .sunset import Sunset
 
+
 class Atmosphere:
     def __repr__(self):
-        '''
+        """
         How should this object appear as a string?
 
         Returns
         -------
         s : str
             A simple string representation.
-        '''
-        scale = (self.H/self.radius).decompose()
-        #H/R={scale},
-        return f'{self.__class__.__name__}Atmosphere ({self.zenith_angle} from zenith, {self.altitude} scale heights from reference)'
+        """
+        scale = (self.H / self.radius).decompose()
+        # H/R={scale},
+        return f"{self.__class__.__name__}Atmosphere ({self.zenith_angle} from zenith, {self.altitude} scale heights from reference)"
 
     # FIXME (maybe both spectrum and atmosphere should inherit from the same thing?)
     def wavelength(self, wavelength=None):
-        '''
+        """
         A wrapper to ensure at least some grid of wavelengths
         gets defined. A default grid will be assumed, unless
         any wavelength array at all is passed.
-        '''
+        """
 
         # make sure at least some wavelengths are defined
         if wavelength is None:
             wavelength = self.default_wavelengths
-        return wavelength.to('nm')
+        return wavelength.to("nm")
 
-    def plot(self,  ax=None,
-                    wavelength=None,
-                    rainbow=True,
-                    color=None,
-                    style='dark_background',
-                    figsize=(5.0, 2.5),
-                    **kwargs):
-        '''
+    def plot(
+        self,
+        ax=None,
+        wavelength=None,
+        rainbow=True,
+        color=None,
+        style="dark_background",
+        figsize=(5.0, 2.5),
+        **kwargs,
+    ):
+        """
         A quick tool to plot the transmission through the atmosphere.
 
         Parameters
         ----------
         ax : matplotlib.axes._subplots.AxesSubplot
             Specify an axes object into which
             this plot should be drawn. This allows
@@ -62,70 +66,70 @@
             Should we add an extra rainbow above the plot,
             to indicate how wavelengths match to visible light?
 
         color : str
             The color for drawing the spectrum.
             'auto' represents the actual visible color.
 
-        '''
+        """
 
         # set up to use a dark background for the plot; make sure units match
         with plt.style.context(style), quantity_support():
 
             # setup the basic axes
             ax = setup_axes_with_rainbow(ax=ax, rainbow=rainbow, figsize=figsize)
 
             # make sure at least some wavelengths are defined
             w = self.wavelength(wavelength)
 
             # pull out the spectrum
             t = self.transmission(w)
 
-            plt.plot(w, t*100, color=color, label=self, **kwargs)
+            plt.plot(w, t * 100, color=color, label=self, **kwargs)
 
             # add the axis labels
-            wunit = w.unit.to_string('latex_inline')
-            plt.xlabel(f'Wavelength ({wunit})')
-            plt.ylabel(f'Transmission (%)')
+            wunit = w.unit.to_string("latex_inline")
+            plt.xlabel(f"Wavelength ({wunit})")
+            plt.ylabel(f"Transmission (%)")
 
             plt.xlim(np.min(w).value, np.max(w).value)
 
         return ax
 
-    def set_elevation_angle(self, elevation=90*u.deg):
-        '''
+    def set_elevation_angle(self, elevation=90 * u.deg):
+        """
         Set the elevation angle above the horizon.
 
         Parameters
         ----------
         elevation : astropy.units.quantity.Quantity
             The angle above the horizon along which
             the transmission of the atmosphere should
             be calculated.
-        '''
-        self.set_zenith_angle(90*u.deg - elevation)
+        """
+        self.set_zenith_angle(90 * u.deg - elevation)
 
-    def set_zenith_angle(self, zenith_angle=0*u.deg):
-        '''
+    def set_zenith_angle(self, zenith_angle=0 * u.deg):
+        """
         Set the angle from zenith.
 
         Parameters
         ----------
         zenith_angle : astropy.units.quantity.Quantity
             The angle away from zenith along which
             the transmission of the atmosphere should
             be calculated.
-        '''
+        """
 
         # set the zenith angle and airmass
-        self.zenith_angle = np.minimum(zenith_angle, 90*u.deg)
-        self.airmass = 1/np.cos(self.zenith_angle)
+        self.zenith_angle = np.minimum(zenith_angle, 90 * u.deg)
+        self.airmass = 1 / np.cos(self.zenith_angle)
 
     def set_altitude(self, altitude=0):
-        '''
+        """
         Set how many atmospheric scale heights we are
         above or below the reference radius of this
         atmosphere.
 
         Parameters
         ----------
         altitude : float
@@ -136,93 +140,105 @@
             transparent atmosphere, and -1.0 is one scale
             height deeper than the reference radius and
             therefore a more opaque atmosphere.
             Negative altitudes are probably a weird concept
             if the reference radius is the surface of a
             rocky planet, but they're quite reasonable
             on gas-dominated planets.
-        '''
+        """
         self.altitude = altitude
-        self.tau_zenith = self._tau_zenith_reference*np.exp(-altitude)
+        self.tau_zenith = self._tau_zenith_reference * np.exp(-altitude)
 
         # guess what is scattering vs. extinction
         self.guess_scattering()
 
     def transmit(self, spectrum):
-        '''
+        """
         Calculate the spectrum of light that results from
         transmitting a known light source through this
         atmosphere.
 
         Parameters
         ----------
         spectrum : Spectrum
             Any light source that you want to transmit.
-        '''
+        """
 
         # create a composite object, linking the source and the atmosphere
         return Sunset(source=spectrum, atmosphere=self)
 
+
 class DiscreteAtmosphere(Atmosphere):
-    '''
+    """
     The DiscreteAtmosphere represents an atmosphere
     whose transmission as a function of wavelength
     can be represented as a grid of zenithward optical
     depths. Most pre-calculated models will fall
     into this category.
-    '''
+    """
 
-    def __init__(self, zenith_angle=0.0*u.deg, altitude=0.0, **kwargs):
-        '''
+    def __init__(self, zenith_angle=0.0 * u.deg, altitude=0.0, **kwargs):
+        """
         In inherited classes, this initialization relies on the
         existence of a method called ".read_transmission"
         that will create the attributes:
             ._wavelengths (with units of wavelength)
             ._tau_zenith_reference (unitless)
             .H (with units of length)
             .radius (with units of length)
-        '''
+        """
 
         # read the transmission spectrum data
         self.read_transmission(**kwargs)
         self.default_wavelengths = self._wavelength
 
         # set the zenith angle (or fall back to the current setting)
         self.set_zenith_angle(zenith_angle)
 
         # set the altitude at which we're hovering
         self.set_altitude(altitude)
 
-
     def guess_scattering(self, visualize=False):
-        '''
+        """
         Make a guess at the Rayleigh scattering component of
         the atmospheric extinction, for use in estimating
         the sky color.
 
         This should be called once per every new altitude.
-        '''
+        """
 
         # figure out the appropriate normalization
-        self._rayleigh_normalization = np.min(self.tau_zenith*self.default_wavelengths**4)
+        self._rayleigh_normalization = np.min(
+            self.tau_zenith * self.default_wavelengths ** 4
+        )
 
         w = self.default_wavelengths
-        self.tau_zenith_scatter = self._rayleigh_normalization/w**4
-        self.tau_zenith_absorb =  self.tau_zenith - self.tau_zenith_scatter
+        self.tau_zenith_scatter = self._rayleigh_normalization / w ** 4
+        self.tau_zenith_absorb = self.tau_zenith - self.tau_zenith_scatter
 
         if visualize:
 
-            plt.plot(w, self.tau_zenith, zorder=100, label='total')
-            plt.plot(w, self.tau_zenith_scatter, alpha=0.5, label='scattering')
-            plt.plot(w, self.tau_zenith_absorb, alpha=0.5, label='absorbtion')
+            plt.plot(w, self.tau_zenith, zorder=100, label="total")
+            plt.plot(
+                w,
+                self.tau_zenith_scatter,
+                alpha=0.5,
+                label="scattering",
+            )
+            plt.plot(
+                w,
+                self.tau_zenith_absorb,
+                alpha=0.5,
+                label="absorbtion",
+            )
             plt.legend()
-            plt.xscale('log')
-            plt.yscale('log')
-            plt.xlabel('Wavelength ({})'.format(w.unit.to_string('latex_inline')))
-            plt.ylabel(r'$\tau_{zenith}$')
+            plt.xscale("log")
+            plt.yscale("log")
+            plt.xlabel("Wavelength ({})".format(w.unit.to_string("latex_inline")))
+            plt.ylabel(r"$\tau_{zenith}$")
 
     """
     def tau_zenith_scatter(self):
         '''
         Estimate the optical depth to *absorption*.
         (at the default wavelengths of the grid)
         '''
@@ -235,68 +251,71 @@
         (at the default wavelengths of the grid)
         '''
         # calculate the extinction from absorption
         return self.tau_zenith - self.tau_zenith_scatter()
     """
 
     def fortney_factor(self):
-        '''
+        """
         The ratio of optical depth between a horizontal slant path
         through an atmosphere to a vertical path, accounting
         for the sphericity of the planet. This is a simple approach
         to connect exoplanet transmission spectra to vertical
         optical depths through an atmosphere (see Fortney 2005).
 
         Returns
         -------
         fortney_factor : float
             The ratio of slant to vertical optical depths.
-        '''
+        """
 
         # calculate the fortney factor = ratio of slant/vertical optical depths
-        return np.sqrt(2*np.pi*self.radius/self.H).decompose()
+        return np.sqrt(2 * np.pi * self.radius / self.H).decompose()
 
     def transit_radius(self, wavelength=None):
-        '''
+        """
         Calculate the effective transit radius of the planet's atmosphere,
         as seen from infinitely far away.
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the transit radius.
 
         Returns
         -------
         transit_radius : astropy.units.quantity.Quantity
             The projected radius of the planet, with units.
-        '''
+        """
         # make sure at least some grid of wavelengths is defined
         w = self.wavelength(wavelength)
 
         # figure out the slant optical depth at the reference radius
         effective_airmass = self.fortney_factor()
-        tau = self._tau_zenith_reference*effective_airmass
+        tau = self._tau_zenith_reference * effective_airmass
 
         # bin this spectrum to the particular wavelength grid
         # KLUDGE -- this should really be in transmission space!
-        neww, tau_slant = bintogrid(self._wavelength.to('nm').value, tau,
-                               newx=w.to('nm').value,
-                               drop_nans=False)
+        neww, tau_slant = bintogrid(
+            self._wavelength.to("nm").value,
+            tau,
+            newx=w.to("nm").value,
+            drop_nans=False,
+        )
 
         # make sure the wavelengths match up
-        assert(np.all(neww == w.to('nm').value))
+        assert np.all(neww == w.to("nm").value)
 
         # convert back to tau
         z_over_H = np.log(tau_slant)
 
-        return self.radius + self.H*z_over_H
+        return self.radius + self.H * z_over_H
 
     def transmission(self, wavelength=None, zenith_angle=None, altitude=None):
-        '''
+        """
         Calculate the transmission through the atmosphere.
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the transmission.
 
@@ -308,36 +327,39 @@
             The altitude at which we should be floating
             in the atmosphere, in units of scale heights.
 
         Returns
         -------
         transmission : numpy.ndarray
             The fractional transmission through the atmosphere.
-        '''
+        """
 
         # update the zenith angle, if necessary
         if zenith_angle is not None:
             self.set_zenith_angle(zenith_angle)
 
         # update the altitude, if necessary
         if altitude is not None:
             self.set_altitude(altitude)
 
         # make sure at least some grid of wavelengths is defined
         w = self.wavelength(wavelength)
 
         # figure out the transmission at this altitude
         # FIXME -- this is a major kludge! do the integral!
-        effective_airmass = np.minimum(self.fortney_factor()/2.0, self.airmass)
-        tau = self.tau_zenith*effective_airmass
+        effective_airmass = np.minimum(self.fortney_factor() / 2.0, self.airmass)
+        tau = self.tau_zenith * effective_airmass
 
         # bin this spectrum to the particular wavelength grid
         # FIXME: binning choice gets real scary with transmission
-        neww, newt = bintogrid(self._wavelength.to('nm').value, np.exp(-tau),
-                         newx=w.to('nm').value,
-                         drop_nans=False)
+        neww, newt = bintogrid(
+            self._wavelength.to("nm").value,
+            np.exp(-tau),
+            newx=w.to("nm").value,
+            drop_nans=False,
+        )
 
         # make sure the wavelengths match up
-        assert(np.all(neww == w.to('nm').value))
+        assert np.all(neww == w.to("nm").value)
 
         # return the binned transmission
         return newt
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/earth.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/earth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from .atmosphere import *
 
+
 class Earth(DiscreteAtmosphere):
-    '''
+    """
     Earth's transmission spectrum.
-    '''
+    """
 
     def read_transmission(self, **kwargs):
-        '''
+        """
         Read Earth's transmission spectrum in from a file
         and define the required attributes:
 
             ._wavelengths (with units of wavelength)
             ._tau_zenith_reference (unitless)
             .H (with units of length)
             .radius (with units of length)
-        '''
+        """
 
         # load the ESO vertical transmission through Earth's atmosphere
-        filename = os.path.join(data_directory, 'earthtransmission.txt')
-        d = ascii.read(filename, comment='#')
-
+        filename = os.path.join(data_directory, "earthtransmission.txt")
+        d = ascii.read(filename, comment="#")
 
         # calculate the optical depth at zenith
-        self._wavelength = d['wavelength'].data*1e3*u.nm
-        self._transmission_zenith = d['transmission'].data
-
+        self._wavelength = d["wavelength"].data * 1e3 * u.nm
+        self._transmission_zenith = d["transmission"].data
 
         # define geometry of the atmosphere (how spherical?)
         mu = 29
-        self.T = 273*u.K
-        g = 9.8*u.m/u.s**2
-        self.H = (con.k_B*self.T/mu/g/con.m_p).to('km')
-        self.radius = 1*u.Rearth
+        self.T = 273 * u.K
+        g = 9.8 * u.m / u.s ** 2
+        self.H = (con.k_B * self.T / mu / g / con.m_p).to("km")
+        self.radius = 1 * u.Rearth
 
         # the file is for Cerro Paranal at 2640m
         # let's move it down to sea level
         tau_zenith_paranal = -np.log(self._transmission_zenith)
-        paranal_altitude = 2640*u.m
-        factor = np.exp(paranal_altitude/self.H)
-        self._tau_zenith_reference = tau_zenith_paranal*factor
+        paranal_altitude = 2640 * u.m
+        factor = np.exp(paranal_altitude / self.H)
+        self._tau_zenith_reference = tau_zenith_paranal * factor
         # to get back to Boulder, set altiude=0.25(=2/8km)
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/exoplanet.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/exoplanet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from .atmosphere import *
 
-class Exoplanet(DiscreteAtmosphere):
 
-    def __init__(self, wavelength, planet_radius, H=20*u.km,
-                       altitude=0.0,
-                       zenith_angle=0.0*u.deg,
-                       **kwargs):
-        '''
+class Exoplanet(DiscreteAtmosphere):
+    def __init__(
+        self,
+        wavelength,
+        planet_radius,
+        H=20 * u.km,
+        altitude=0.0,
+        zenith_angle=0.0 * u.deg,
+        **kwargs
+    ):
+        """
         Initialize a generic exoplanet atmosphere from a model exoplanet
         transmission spectrum, specified by the inputs `wavelength`
         and `planet_radius`
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
@@ -26,35 +31,33 @@
         altitude : float
             The altitude at which we should be floating
             in the atmosphere, in units of scale heights.
         zenith_angle : astropy.units.quantity.Quantity
             The default angle from zenith along which transmission
             should be calculated (this can be changed).
 
-        '''
-
+        """
 
         # define the wavelength grid
-        self._wavelength = wavelength.to('nm')
+        self._wavelength = wavelength.to("nm")
 
         # store the effective transit radius
         self._transit_radius = planet_radius
 
         # pick an (arbitrary-ish) reference radius
         reference_radius = np.min(self._transit_radius)
 
         # define geometry of the atmosphere (how spherical?)
         self.H = H
         self.radius = reference_radius
 
         # calculate the optical depth at zenith
-        z_over_H = ((self._transit_radius - reference_radius)/self.H).decompose()
+        z_over_H = ((self._transit_radius - reference_radius) / self.H).decompose()
         tau_slant = np.exp(z_over_H)
-        self._tau_zenith_reference = (tau_slant/self.fortney_factor()).decompose()
-
+        self._tau_zenith_reference = (tau_slant / self.fortney_factor()).decompose()
 
         # define the default wavelength grid to use
         self.default_wavelengths = self._wavelength
 
         # set the zenith angle (or fall back to the current setting)
         self.set_zenith_angle(zenith_angle)
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/hotjupiter.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/hotjupiter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from .atmosphere import *
 
-class HotJupiter(DiscreteAtmosphere):
 
+class HotJupiter(DiscreteAtmosphere):
     def read_transmission(self, TiO=False, **kwargs):
-        '''
+        """
         Read a Hot Jupiter's transmission spectrum in from a file
         and define the required attributes:
 
             ._wavelengths (with units of wavelength)
             ._tau_zenith_reference (unitless)
             .H (with units of length)
             .radius (with units of length)
-        '''
+        """
 
         # load a transmission spectrum from Fortney et al. (2010)
         if TiO:
-            choice = 'lambda_1500K_g10_wTiOVO.dat'
+            choice = "lambda_1500K_g10_wTiOVO.dat"
         else:
-            choice = 'lambda_1500K_g10_noTiOVO.dat'
-        filename = os.path.join(data_directory, f'fortney/{choice}')
-        d = ascii.read(filename, comment='#')
+            choice = "lambda_1500K_g10_noTiOVO.dat"
+        filename = os.path.join(data_directory, f"fortney/{choice}")
+        d = ascii.read(filename, comment="#")
 
         # define the wavelength grid
-        self._wavelength = d['wavelength'].data*1e3*u.nm
+        self._wavelength = d["wavelength"].data * 1e3 * u.nm
 
         # store the effective transit radius
-        radiusinkm = d['radiusinkm'].data*u.km
-        self._transit_radius = radiusinkm.to('Rjup')
+        radiusinkm = d["radiusinkm"].data * u.km
+        self._transit_radius = radiusinkm.to("Rjup")
 
         # pick an (arbitrary-ish) reference radius
         reference_radius = np.min(radiusinkm)
 
         # define geometry of the atmosphere (how spherical?)
         mu = 2.3
-        self.T = 1500*u.K
-        g = 10*u.m/u.s**2
-        self.H = (con.k_B*self.T/mu/g/con.m_p).to('km')
+        self.T = 1500 * u.K
+        g = 10 * u.m / u.s ** 2
+        self.H = (con.k_B * self.T / mu / g / con.m_p).to("km")
         self.radius = reference_radius
 
         # calculate the optical depth at zenith
-        z_over_H = ((radiusinkm - reference_radius)/self.H).decompose()
+        z_over_H = ((radiusinkm - reference_radius) / self.H).decompose()
         tau_slant = np.exp(z_over_H)
-        self._tau_zenith_reference = (tau_slant/self.fortney_factor()).decompose()
+        self._tau_zenith_reference = (tau_slant / self.fortney_factor()).decompose()
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/noatmosphere.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/noatmosphere.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from .atmosphere import *
 
+
 class NoAtmosphere(Atmosphere):
-    '''
+    """
     A fake atmosphere that represents a completely transparent atmosphere.
     This might be useful as a placeholder, if you want to make
     plots/animations that directly compare the spectrum of a
     source with or without extinction by an atmosphere.
-    '''
+    """
 
     def __repr__(self):
-        '''
+        """
         How should this object appear as a string?
 
         Returns
         -------
         s : str
             A simple string representation.
-        '''
-        #H/R={scale},
-        return f'{self.__class__.__name__}Atmosphere'
-
+        """
+        # H/R={scale},
+        return f"{self.__class__.__name__}Atmosphere"
 
-    def __init__(self, zenith_angle=0.0*u.deg, **kwargs):
-        '''
+    def __init__(self, zenith_angle=0.0 * u.deg, **kwargs):
+        """
         Initialize the fake atmosphereless atmosphere.
-        '''
+        """
 
         # read the transmission spectrum data
-        self.default_wavelengths = np.arange(300, 1000, 1)*u.nm
+        self.default_wavelengths = np.arange(300, 1000, 1) * u.nm
 
         # set the zenith angle (or fall back to the current setting)
         self.set_zenith_angle(zenith_angle)
 
     def transmission(self, wavelength=None, zenith_angle=None, **kw):
-        '''
+        """
         Calculate the transmission through the atmosphere.
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the transmission.
 
@@ -45,15 +45,15 @@
             The angle from zenith along which transmission
             should be calculated.
 
         Returns
         -------
         transmission : numpy.ndarray
             The fractional transmission through the atmosphere.
-        '''
+        """
 
         # update the zenith angle, if necessary
         if zenith_angle is not None:
             self.set_zenith_angle(zenith_angle)
 
         # make sure at least some grid of wavelengths is defined
         w = self.wavelength(wavelength)
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/sky.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/sky.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 from ..imports import *
 from ..sources import Spectrum, Thermal
 from colour.phenomena.rayleigh import rayleigh_optical_depth
 
-class Sky(Spectrum):
 
+class Sky(Spectrum):
     def __init__(self, sunset):
-        '''
+        """
         Initialize this composite object, connecting a light source
         and an atmosphere together into a diffuse Sky calculator.
 
         Parameters
         ----------
         sunset : rainbowconnection.Sunset
             Any object with both a source and an atmosphere.
             Calculations related to the diffuse sky brightness
             require both, so it's simplest just to pass
             a sunset object in which they are already linked.
-        '''
+        """
 
         self.sunset = sunset
         self.source = sunset.source
         self.atmosphere = sunset.atmosphere
 
         try:
             self.B = Thermal(self.atmosphere.T).intensity
         except AttributeError:
+
             def f(wavelength):
-                return np.zeros(np.shape(wavelength))*u.W/u.m**2/u.nm*u.sr
+                return np.zeros(np.shape(wavelength)) * u.W / u.m ** 2 / u.nm * u.sr
+
             self.B = f
 
-        self.set_zenith_angle(0*u.deg)
+        self.set_zenith_angle(0 * u.deg)
         # self.is_earth = 'Earth' in self.atmosphere.__class__.__name__
 
-
-    def set_zenith_angle(self, zenith_angle=0*u.deg):
-        '''
+    def set_zenith_angle(self, zenith_angle=0 * u.deg):
+        """
         Set the angle from zenith (for a slice of the sky.)
 
         Parameters
         ----------
         zenith_angle : astropy.units.quantity.Quantity
             The angle away from zenith along which
             the transmission of the atmosphere should
             be calculated.
-        '''
+        """
 
         # set the zenith angle and airmass
-        self.zenith_angle = np.minimum(zenith_angle, 90*u.deg)
-        self.airmass = 1/np.cos(self.zenith_angle)
-
+        self.zenith_angle = np.minimum(zenith_angle, 90 * u.deg)
+        self.airmass = 1 / np.cos(self.zenith_angle)
 
     def spectrum(self, wavelength=None):
-        '''
+        """
         Calculate intensity of the diffuse sky at a given zenith angle.
         Currently this accounts only for Rayleigh scattering (assuming
         perfect 1/wavelength**4) and for thermal emission (which is
         usually negligible below about 1700K). The relative contributions
         of scattering and aborption/emission are estimated in a very
         cartoonish fashion from the overall extinction, and assumes
         there is at least one wavelength in the spectrum that is
         dominated by scattering.
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the spectrum.
-        '''
-
+        """
 
         # figure out the airmass along this line of sight
         # airmass = 1/np.cos(self.zenith_angle)
-        effective_airmass = np.minimum(self.atmosphere.fortney_factor()/2.0,
-                                       self.airmass)
-
+        effective_airmass = np.minimum(
+            self.atmosphere.fortney_factor() / 2.0, self.airmass
+        )
 
         # calculate the optical depths at this angle
-        tau_scatter = self.atmosphere.tau_zenith_scatter*effective_airmass
-        tau_absorb = self.atmosphere.tau_zenith_absorb*effective_airmass
+        tau_scatter = self.atmosphere.tau_zenith_scatter * effective_airmass
+        tau_absorb = self.atmosphere.tau_zenith_absorb * effective_airmass
 
         # estimate the single
-        albedo = tau_scatter/(tau_absorb + tau_scatter)
+        albedo = tau_scatter / (tau_absorb + tau_scatter)
 
         # calculate the mean intensity field
         mean_intensity = self.sunset.mean_intensity()
 
         # calculate the intensity of the illuminated sky (away from the disk)
-        thermal_intensity = (1 - albedo)*self.B(self.atmosphere.default_wavelengths)*(1 - np.exp(-tau_absorb))
-        scattering_intensity = albedo * mean_intensity*(1 - np.exp(-tau_scatter))
+        thermal_intensity = (
+            (1 - albedo)
+            * self.B(self.atmosphere.default_wavelengths)
+            * (1 - np.exp(-tau_absorb))
+        )
+        scattering_intensity = albedo * mean_intensity * (1 - np.exp(-tau_scatter))
         sky_intensity = thermal_intensity + scattering_intensity
 
         # bin this intensity onto the desired wavelengths
         w = self.wavelength(wavelength)
         unit = sky_intensity.unit
-        neww, newi = bintogrid(self.atmosphere.default_wavelengths, sky_intensity.value,
-                         newx=w.to('nm').value,
-                         drop_nans=False)
+        neww, newi = bintogrid(
+            self.atmosphere.default_wavelengths,
+            sky_intensity.value,
+            newx=w.to("nm").value,
+            drop_nans=False,
+        )
 
         # make sure the wavelengths match up
-        assert(np.all(neww == w.to('nm').value))
-
+        assert np.all(neww == w.to("nm").value)
 
         # return this sky intensity
-        return newi*unit
+        return newi * unit
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/atmospheres/sunset.py` & `rainbow-connection-0.0.7/rainbowconnection/atmospheres/sunset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ..imports import *
 from ..sources import Spectrum
 from ..animatetools import *
 from .sky import *
 
-class Sunset(Spectrum):
 
+class Sunset(Spectrum):
     def __init__(self, source, atmosphere):
-        '''
+        """
         Initialize this composite object, connecting a light source
         and an atmosphere together into a Sunset calculator.
 
         Parameters
         ----------
         source : rainbowconnection.Spectrum
             The light source from above the atmosphere.
         atmosphere : rainbowconnection.Atmosphere
             The atmosphere through which the light source propagates.
-        '''
+        """
 
         self.source = source
         self.atmosphere = atmosphere
         self.sky = Sky(self)
 
     # KLUDGE - there's got to be a better way to organize this?!
     @property
@@ -32,36 +32,36 @@
     def distance(self):
         try:
             return self.source.distance
         except AttributeError:
             return None
 
     def __repr__(self):
-        '''
+        """
         How should this be represented as a string?
-        '''
+        """
 
         s = repr(self.source)
         t = repr(self.atmosphere)
-        return f'{s}\n through\n{t}'
+        return f"{s}\n through\n{t}"
 
     def set_zenith_angle(self, *args, **kwargs):
-        '''
+        """
         Pass zenith commands up to the atmosphere.
-        '''
+        """
         self.atmosphere.set_zenith_angle(*args, **kwargs)
 
     def set_altiude(self, *args, **kwargs):
-        '''
+        """
         Pass altitude commands up to the atmosphere.
-        '''
+        """
         self.atmosphere.set_altitude(*args, **kwargs)
 
     def spectrum(self, wavelength=None, zenith_angle=None, altitude=None):
-        '''
+        """
         The spectrum of the light source viewed through the atmosphere.
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the spectrum.
 
@@ -74,99 +74,113 @@
             The altitude at which we should be floating
             in the atmosphere, in units of scale heights.
 
         Returns
         -------
         spectrum : astropy.units.quantity.Quantity
             The luminosity (W/nm) or flux (W/nm/m**2).
-        '''
+        """
 
         # the transmission wavelength sets the grid
         w = self.atmosphere.wavelength(wavelength)
 
         # get the transmission a
-        t = self.atmosphere.transmission(wavelength=w,
-                                         zenith_angle=zenith_angle,
-                                         altitude=altitude)
+        t = self.atmosphere.transmission(
+            wavelength=w,
+            zenith_angle=zenith_angle,
+            altitude=altitude,
+        )
 
         # get the original spectrum
         s = self.source.spectrum(wavelength=w)
 
         # return the transmitted spectrum
-        return s*t
+        return s * t
 
     def transit_depth(self, wavelength=None):
-        '''
+        """
         The transit depth of the planet, passing in front of the light source.
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the spectrum.
 
         Returns
         -------
         transitdepth : np.ndarry
             The fraction of starlight blocked, unitless.
-        '''
+        """
 
         # the transmission wavelength sets the grid
         w = self.atmosphere.wavelength(wavelength)
 
         # get the transmission a
         rp = self.atmosphere.transit_radius(wavelength=w)
 
         # get the original spectrum
         rs = self.source.radius
 
-        return (rp/rs).decompose()**2
+        return (rp / rs).decompose() ** 2
 
-
-    def plot_disk(self, ax=None, zenith_angle=89*u.deg, azimuth_angle=0*u.deg):
-        '''
+    def plot_disk(
+        self,
+        ax=None,
+        zenith_angle=89 * u.deg,
+        azimuth_angle=0 * u.deg,
+    ):
+        """
         Plot the disk of the star.
 
         Parameters
         ----------
         ax : matplotlib.axes._subplots.AxesSubplot
             The axes into which this plot should be drawn.
         zenith_angle : astropy.units.quantity.Quantity
             The angle away from zenith.
         azimuth_angle : astropy.units.quantity.Quantity
             The azimuth angle along the horizon.
-        '''
+        """
 
-        with plt.style.context('dark_background'), quantity_support():
+        with plt.style.context("dark_background"), quantity_support():
 
             if ax is not None:
                 plt.sca(ax)
 
             # set the zenith angle
             self.set_zenith_angle(zenith_angle)
 
             # figure out the color of the star
             rgb = self.to_color()
 
-            c = plt.Circle(xy=[azimuth_angle, 90*u.deg - zenith_angle],
-                           radius=self.source.angular_size(),
-                           facecolor=rgb, zorder=1000)
+            c = plt.Circle(
+                xy=[azimuth_angle, 90 * u.deg - zenith_angle],
+                radius=self.source.angular_size(),
+                facecolor=rgb,
+                zorder=1000,
+            )
             plt.gca().add_patch(c)
 
-            size = self.source.angular_size()*1.1
+            size = self.source.angular_size() * 1.1
             plt.xlim(azimuth_angle - size, azimuth_angle + size)
-            plt.ylim(90*u.deg - zenith_angle - size,
-                     90*u.deg - zenith_angle + size)
-            plt.axis('scaled')
+            plt.ylim(
+                90 * u.deg - zenith_angle - size,
+                90 * u.deg - zenith_angle + size,
+            )
+            plt.axis("scaled")
             return c
 
-    def plot_sky(self, maxelevation=20*u.deg,
-                       minelevation=0*u.deg,
-                       skyresolution=0.5*u.deg,
-                       skynormalization=0.7):
-        '''
+    def plot_sky(
+        self,
+        maxelevation=20 * u.deg,
+        minelevation=0 * u.deg,
+        skyresolution=0.5 * u.deg,
+        skynormalization=0.7,
+    ):
+        """
         Plot a diffuse sky behind the disk of the star.
 
         Parameters
         ----------
         maxelevation : astropy.units.quantity.Quantity
             The maximum elevation above the horizon.
         minelevation : astropy.units.quantity.Quantity
@@ -179,51 +193,61 @@
         skynormalization : float
             By what factor do we down-weight the intensity
             of the sky. To be quantitatively correct, this
             should be something like the ratio of the
             stellar disk intensity to the diffuse sky
             brightness, but that factor is so tiny that
             the sky would always seem to be black.
-        '''
+        """
 
-        if self.atmosphere.__class__.__name__== 'NoAtmosphere':
+        if self.atmosphere.__class__.__name__ == "NoAtmosphere":
             return
 
         # set the elevations where we will calculate sky colors
-        elevations = np.arange(minelevation.to('deg').value,
-                               (maxelevation + skyresolution).to('deg').value,
-                               skyresolution.to('deg').value)*u.deg
+        elevations = (
+            np.arange(
+                minelevation.to("deg").value,
+                (maxelevation + skyresolution).to("deg").value,
+                skyresolution.to("deg").value,
+            )
+            * u.deg
+        )
 
         # calculate a list of sky colors, one for each elevation
         colors = []
         for e in elevations:
 
             # point at a particular stripe of the sky
-            self.sky.set_zenith_angle(90*u.deg - e)
+            self.sky.set_zenith_angle(90 * u.deg - e)
 
             # estimate the color of that stripe
-            colors.append(self.sky.to_color()*skynormalization)
+            colors.append(self.sky.to_color() * skynormalization)
 
         # draw horizontal bars with these colors
-        plt.barh(y=elevations,
-                 width=20,
-                 height=skyresolution,
-                 left=-10,
-                 zorder=-100,
-                 color=colors)
-
-    def plot_sunset(self, ax=None,
-                          zenith_angle=89*u.deg,
-                          azimuth_angle=0*u.deg,
-                          maxelevation=20*u.deg,
-                          minelevation=-5*u.deg,
-                          skyresolution=0.5*u.deg,
-                          skynormalization=0.7):
+        plt.barh(
+            y=elevations,
+            width=20,
+            height=skyresolution,
+            left=-10,
+            zorder=-100,
+            color=colors,
+        )
+
+    def plot_sunset(
+        self,
+        ax=None,
+        zenith_angle=89 * u.deg,
+        azimuth_angle=0 * u.deg,
+        maxelevation=20 * u.deg,
+        minelevation=-5 * u.deg,
+        skyresolution=0.5 * u.deg,
+        skynormalization=0.7,
+    ):
 
-        '''
+        """
         Plot the disk of the star and the diffuse sky.
 
         Parameters
         ----------
         ax : matplotlib.axes._subplots.AxesSubplot
             The axes into which this plot should be drawn.
         zenith_angle : astropy.units.quantity.Quantity
@@ -242,48 +266,55 @@
         skynormalization : float
             By what factor do we down-weight the intensity
             of the sky. To be quantitatively correct, this
             should be something like the ratio of the
             stellar disk intensity to the diffuse sky
             brightness, but that factor is so tiny that
             the sky would always seem to be black.
-        '''
+        """
 
         # make sure we're using a dark background and astropy units
-        with plt.style.context('dark_background'), quantity_support():
+        with plt.style.context("dark_background"), quantity_support():
 
             if ax is not None:
                 plt.sca(ax)
 
             # put the sun at a particular elevation
             self.set_zenith_angle(zenith_angle)
 
             # plot the diffuse sky
-            self.plot_sky(maxelevation=maxelevation,
-                          minelevation=minelevation)
+            self.plot_sky(
+                maxelevation=maxelevation,
+                minelevation=minelevation,
+            )
 
             # plot the disk of the sun
-            self.plot_disk(zenith_angle=zenith_angle,
-                           azimuth_angle=azimuth_angle)
+            self.plot_disk(
+                zenith_angle=zenith_angle,
+                azimuth_angle=azimuth_angle,
+            )
 
             # fuss with the axis labels
-            plt.axis('scaled')
-            plt.xlim(-5*u.deg, 5*u.deg)
-            plt.ylim(0*u.deg, maxelevation)
-            plt.ylabel('Angle above Horizon')
+            plt.axis("scaled")
+            plt.xlim(-5 * u.deg, 5 * u.deg)
+            plt.ylim(0 * u.deg, maxelevation)
+            plt.ylabel("Angle above Horizon")
             ax = plt.gca()
             ax.get_xaxis().set_visible(False)
         return ax
 
-    def animate_sunset(self, filename='sunset.mp4',
-                             maxelevation=30*u.deg,
-                             skyresolution=0.5*u.deg,
-                             skynormalization=0.7,
-                             motionresolution=0.5*u.deg):
-        '''
+    def animate_sunset(
+        self,
+        filename="sunset.mp4",
+        maxelevation=30 * u.deg,
+        skyresolution=0.5 * u.deg,
+        skynormalization=0.7,
+        motionresolution=0.5 * u.deg,
+    ):
+        """
         Animate the sun setting.
 
         Parameters
         ----------
         filename : string
             The filename where this animation should be saved
         maxelevation : astropy.units.quantity.Quantity
@@ -299,62 +330,70 @@
             should be something like the ratio of the
             stellar disk intensity to the diffuse sky
             brightness, but that factor is so tiny that
             the sky would always seem to be black.
         motionresolution : astropy.units.quantity.Quantity
             The angular step the star moves between
             frames of the animation.
-        '''
-
+        """
 
         # get the appropriate animation writer
         wri = get_writer(filename)
 
         # calculate the grid of zenith angles for the star
-        min_zenith = 90*u.deg - maxelevation - self.source.angular_size()
+        min_zenith = 90 * u.deg - maxelevation - self.source.angular_size()
         minelevation = -(self.source.angular_size() + motionresolution)
-        max_zenith = 90*u.deg - minelevation
-        zenith_angles = np.arange(min_zenith.to('deg').value,
-                                  max_zenith.to('deg').value,
-                                  motionresolution.to('deg').value)*u.deg
-
+        max_zenith = 90 * u.deg - minelevation
+        zenith_angles = (
+            np.arange(
+                min_zenith.to("deg").value,
+                max_zenith.to("deg").value,
+                motionresolution.to("deg").value,
+            )
+            * u.deg
+        )
 
         # make a figure with a dark background
-        with plt.style.context('dark_background'), quantity_support():
+        with plt.style.context("dark_background"), quantity_support():
 
             # create a new figure
-            fi, ax = plt.subplots(1,1)
+            fi, ax = plt.subplots(1, 1)
 
             # save to frames of an animation
             with wri.saving(fi, filename, 400):
 
                 # loop over zenith angles
                 for z in tqdm(zenith_angles):
 
                     # clear whatever was in the previous axes
                     ax.cla()
 
                     # plot the sunset at this current stellar zenith angle
-                    self.plot_sunset(ax=ax,
-                                     zenith_angle=z,
-                                     maxelevation=maxelevation,
-                                     minelevation=minelevation)
+                    self.plot_sunset(
+                        ax=ax,
+                        zenith_angle=z,
+                        maxelevation=maxelevation,
+                        minelevation=minelevation,
+                    )
 
                     # grab this frame in the animation
                     wri.grab_frame()
 
-    def animate_everything(self, filename='everything-sunset.mp4',
-                                 ingredients=['sky', 'sky-zoom', 'rgb', 'spectrum'],
-                                 maxelevation=50*u.deg,
-                                 skyresolution=0.5*u.deg,
-                                 skynormalization=0.7,
-                                 motionresolution=0.5*u.deg,
-                                 **kwargs):
+    def animate_everything(
+        self,
+        filename="everything-sunset.mp4",
+        ingredients=["sky", "sky-zoom", "rgb", "spectrum"],
+        maxelevation=50 * u.deg,
+        skyresolution=0.5 * u.deg,
+        skynormalization=0.7,
+        motionresolution=0.5 * u.deg,
+        **kwargs,
+    ):
 
-        '''
+        """
         Make an animation that summarizes
         lots of information about a sunset.
 
         Parameters
         ----------
         filename : string
             The filename where this animation should be saved
@@ -381,58 +420,67 @@
             the sky would always seem to be black.
         motionresolution : astropy.units.quantity.Quantity
             The angular step the star moves between
             frames of the animation.
         **kwargs : dict
             All extra keyword arguments will be passed to
             plot_everything.
-        '''
-
+        """
 
         # get the appropriate animation writer
         wri = get_writer(filename)
 
         # calculate the grid of zenith angles for the star
-        min_zenith = 90*u.deg - maxelevation - self.source.angular_size()
+        min_zenith = 90 * u.deg - maxelevation - self.source.angular_size()
         minelevation = -(self.source.angular_size() + motionresolution)
-        max_zenith = 90*u.deg - minelevation
-        zenith_angles = np.arange(min_zenith.to('deg').value,
-                                  max_zenith.to('deg').value,
-                                  motionresolution.to('deg').value)*u.deg
+        max_zenith = 90 * u.deg - minelevation
+        zenith_angles = (
+            np.arange(
+                min_zenith.to("deg").value,
+                max_zenith.to("deg").value,
+                motionresolution.to("deg").value,
+            )
+            * u.deg
+        )
 
-        with plt.style.context('dark_background'), quantity_support():
+        with plt.style.context("dark_background"), quantity_support():
 
             fi = self.plot_everything(zenith_angles[0], **kwargs)
 
             # save to frames of an animation
             with wri.saving(fi, filename, fi.get_dpi()):
 
                 # loop over zenith angles
                 for z in tqdm(zenith_angles):
 
                     # clear whatever was in the previous axes
                     fi.clf()
 
                     # plot the sunset at this current stellar zenith angle
-                    self.plot_everything(fi=fi, zenith_angle=z,
-                                         ingredients=ingredients, **kwargs)
+                    self.plot_everything(
+                        fi=fi,
+                        zenith_angle=z,
+                        ingredients=ingredients,
+                        **kwargs,
+                    )
 
                     # grab this frame in the animation
                     wri.grab_frame()
 
-
-    def plot_everything(self, ingredients=['sky', 'sky-zoom', 'rgb', 'spectrum'],
-                              zenith_angle=85*u.deg,
-                              maxelevation=50*u.deg,
-                              fi=None,
-                              pixels=[1920, 1080],
-                              width=8,
-                              filename=None,
-                              ):
-        '''
+    def plot_everything(
+        self,
+        ingredients=["sky", "sky-zoom", "rgb", "spectrum"],
+        zenith_angle=85 * u.deg,
+        maxelevation=50 * u.deg,
+        fi=None,
+        pixels=[1920, 1080],
+        width=8,
+        filename=None,
+    ):
+        """
         Make an animation that summarizes
         lots of information about a sunset.
 
         Parameters
         ----------
         ingredients : list
             The components to draw. These are:
@@ -445,87 +493,108 @@
             The angle away from zenith.
         maxelevation : astropy.units.quantity.Quantity
             The maximum elevation above the horizon
             (for setting the plot limits.)
         aspect : list
             The aspect ratio [width, height] of the
             size of the plot.
-        '''
+        """
 
-        with plt.style.context('dark_background'), quantity_support():
+        with plt.style.context("dark_background"), quantity_support():
             xpixels, ypixels = pixels
-            dpi = xpixels/width
-            scale = 12/width
+            dpi = xpixels / width
+            scale = 12 / width
             if fi is None:
 
-                fi = plt.figure(figsize=(width, ypixels*width/xpixels),
-                                dpi=dpi)
+                fi = plt.figure(
+                    figsize=(width, ypixels * width / xpixels),
+                    dpi=dpi,
+                )
 
             # set up the basic columns
-            gs = GridSpec(  1, 4,
-                            width_ratios=[0.18, 0.4, 0.09*scale,  0.9],
-                            wspace=0.0)
+            gs = GridSpec(
+                1,
+                4,
+                width_ratios=[0.18, 0.4, 0.09 * scale, 0.9],
+                wspace=0.0,
+            )
 
             ax = {}
 
             # set up the contextualizing plots on the left
-            gs_geometry = GridSpecFromSubplotSpec(2, 1,
-                                                  height_ratios=[1, 1],
-                                                  hspace=0.5*scale,
-                                                  subplot_spec=gs[1])
-
-            #ax['cartoon'] = plt.subplot(gs_geometry[0])
-            if 'sky-zoom' in ingredients:
-                ax['sky-zoom'] = plt.subplot(gs_geometry[0])
-                self.plot_disk(ax=ax['sky-zoom'], zenith_angle=zenith_angle)
-                width = 1.1*self.source.angular_size()
+            gs_geometry = GridSpecFromSubplotSpec(
+                2,
+                1,
+                height_ratios=[1, 1],
+                hspace=0.5 * scale,
+                subplot_spec=gs[1],
+            )
+
+            # ax['cartoon'] = plt.subplot(gs_geometry[0])
+            if "sky-zoom" in ingredients:
+                ax["sky-zoom"] = plt.subplot(gs_geometry[0])
+                self.plot_disk(ax=ax["sky-zoom"], zenith_angle=zenith_angle)
+                width = 1.1 * self.source.angular_size()
                 plt.xlim(-width, width)
-                plt.ylim(90*u.deg - zenith_angle - width, 90*u.deg - zenith_angle + width)
-                ax['sky-zoom'].get_xaxis().set_visible(False)
-                ax['sky-zoom'].get_yaxis().set_visible(False)
-                plt.axis('scaled')
-                plt.axis('off')
+                plt.ylim(
+                    90 * u.deg - zenith_angle - width,
+                    90 * u.deg - zenith_angle + width,
+                )
+                ax["sky-zoom"].get_xaxis().set_visible(False)
+                ax["sky-zoom"].get_yaxis().set_visible(False)
+                plt.axis("scaled")
+                plt.axis("off")
 
             # set up the main panel showing the sunset over the full sky
-            if 'sky' in ingredients:
-                ax['sky'] = plt.subplot(gs[0])
+            if "sky" in ingredients:
+                ax["sky"] = plt.subplot(gs[0])
                 # actually make the plots
-                self.plot_sunset(ax=ax['sky'], zenith_angle=zenith_angle, maxelevation=maxelevation)
+                self.plot_sunset(
+                    ax=ax["sky"],
+                    zenith_angle=zenith_angle,
+                    maxelevation=maxelevation,
+                )
 
             #
             # set up the spectrum panels
-            gs_spectra = GridSpecFromSubplotSpec(2, 1,
-                                                 height_ratios=[1, 1],
-                                                 subplot_spec=gs[3],
-                                                 hspace=0.5*scale)
-            if 'rgb' in ingredients:
-                ax['rgb'] = plt.subplot(gs_spectra[0])
-                self.plot_rgb(ax=ax['rgb'])
+            gs_spectra = GridSpecFromSubplotSpec(
+                2,
+                1,
+                height_ratios=[1, 1],
+                subplot_spec=gs[3],
+                hspace=0.5 * scale,
+            )
+            if "rgb" in ingredients:
+                ax["rgb"] = plt.subplot(gs_spectra[0])
+                self.plot_rgb(ax=ax["rgb"])
                 plt.ylim(0, 120)
-                plt.xlim(360*u.nm, 740*u.nm)
+                plt.xlim(360 * u.nm, 740 * u.nm)
 
-            if 'spectrum' in ingredients:
-                ax['spectrum'] = plt.subplot(gs_spectra[1],
-                                             sharex=ax['rgb'], sharey=ax['rgb'])
-                self.plot_as_rainbow(ax['spectrum'])
+            if "spectrum" in ingredients:
+                ax["spectrum"] = plt.subplot(
+                    gs_spectra[1],
+                    sharex=ax["rgb"],
+                    sharey=ax["rgb"],
+                )
+                self.plot_as_rainbow(ax["spectrum"])
                 plt.ylim(0, 120)
-                plt.xlim(360*u.nm, 740*u.nm)
+                plt.xlim(360 * u.nm, 740 * u.nm)
 
         if filename is not None:
-            plt.savefig(filename, facecolor='black')
+            plt.savefig(filename, facecolor="black")
         return fi
 
     def plot_rgb(self, ax=None, **kwargs):
-        '''
+        """
         Wrapper to add the unextincted spectrum
         in dark gray in the background for context.
-        '''
+        """
         ax = Spectrum.plot_rgb(self, ax=ax, **kwargs)
         self.source.plot_rgb(foreground=False, ax=ax)
 
     def plot_as_rainbow(self, ax=None, **kwargs):
-        '''
+        """
         Wrapper to add the unextincted spectrum
         in dark gray in the background for context.
-        '''
+        """
         ax = Spectrum.plot_as_rainbow(self, ax=ax, **kwargs)
         self.source.plot_as_rainbow(foreground=False, ax=ax)
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/colortools.py` & `rainbow-connection-0.0.7/rainbowconnection/colortools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,66 @@
-'''
+"""
 These tools are pulled *very* strongly from the great
 ingredients in the `colour` package. They've been
 modified and simplified here, in order to work better
 with the design of rainbowconnection.
-'''
+"""
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.patches import Polygon
 from six.moves import reduce
 
 from colour.algebra import LinearInterpolator
 from colour.colorimetry import (
-    ILLUMINANTS, ILLUMINANTS_SDS, LIGHTNESS_METHODS, LUMINANCE_METHODS,
-    SpectralShape, sd_blackbody, sd_ones, sd_to_XYZ,
-    wavelength_to_XYZ)
+    CCS_ILLUMINANTS,
+    SDS_ILLUMINANTS,
+    LIGHTNESS_METHODS,
+    LUMINANCE_METHODS,
+    SpectralShape,
+    sd_blackbody,
+    sd_ones,
+    sd_to_XYZ,
+    wavelength_to_XYZ,
+)
 from colour.plotting import (
-    ColourSwatch, COLOUR_STYLE_CONSTANTS, XYZ_to_plotting_colourspace, artist,
-    filter_passthrough, filter_cmfs, filter_illuminants, override_style,
-    render, plot_single_colour_swatch, plot_multi_functions, plot_single_sd)
-from colour.utilities import (domain_range_scale, first_item,
-                              normalise_maximum, tstack)
+    ColourSwatch,
+    CONSTANTS_COLOUR_STYLE,
+    XYZ_to_plotting_colourspace,
+    artist,
+    filter_passthrough,
+    filter_cmfs,
+    filter_illuminants,
+    override_style,
+    render,
+    plot_single_colour_swatch,
+    plot_multi_functions,
+    plot_single_sd,
+)
+from colour.utilities import (
+    domain_range_scale,
+    first_item,
+    normalise_maximum,
+    tstack,
+    ColourRuntimeWarning,
+)
 
 from colour import SpectralDistribution
 
 # define a standard set of color-matching functions
-CMFs = first_item(filter_cmfs('CIE 1931 2 Degree Standard Observer').values())
+CMFs = first_item(filter_cmfs("CIE 1931 2 Degree Standard Observer").values())
 
-def plot_rainbow(axes=None,
-                 wavelength=None, flux=None,
-                 cmfs='CIE 1931 2 Degree Standard Observer',
-                 **kwargs):
+
+def plot_simple_rainbow(
+    ax=None,
+    wavelength=None,
+    flux=None,
+    cmfs="CIE 1931 2 Degree Standard Observer",
+    **kwargs
+):
     """
     Plot a simple horizontal rainbow,
     based off colour's plot_single_sd.
 
     Parameters
     ----------
     ax : matplotlib.axes._subplots.AxesSubplot
@@ -44,73 +70,80 @@
 
     Returns
     -------
     ax : matplotlib.axes._subplots.AxesSubplot
         The ax into which the rainbow was drawn.
     """
 
-    if axes is None:
-        axes = plt.gca()
+    if ax is None:
+        ax = plt.gca()
 
     # pull out the CMFss
     cmfs = first_item(filter_cmfs(cmfs).values())
 
     if wavelength is None:
         # create a grid of wavelengths (at which CMFss are useful)
         wavelength = cmfs.wavelengths
 
-    ok = ((wavelength >= np.min(cmfs.wavelengths)) &
-          (wavelength <= np.max(cmfs.wavelengths)))
+    ok = (wavelength >= np.min(cmfs.wavelengths)) & (
+        wavelength <= np.max(cmfs.wavelengths)
+    )
 
     # create colors at theose wavelengths
     colours = XYZ_to_plotting_colourspace(
         wavelength_to_XYZ(wavelength[ok], cmfs),
-        ILLUMINANTS['CIE 1931 2 Degree Standard Observer']['E'])
-        #apply_encoding_cctf=False)
+        CCS_ILLUMINANTS["CIE 1931 2 Degree Standard Observer"]["E"],
+    )
 
     # normalize the colors to their maximum?
-    colours = COLOUR_STYLE_CONSTANTS.colour.colourspace.encoding_cctf(
-        normalise_maximum(colours))
+    colours = CONSTANTS_COLOUR_STYLE.colour.colourspace.cctf_encoding(
+        normalise_maximum(colours)
+    )
 
     # create y values that will be plotted (these could be spectrum)
     if flux is None:
         flux = np.ones_like(wavelength)
     x_min, x_max = min(wavelength), max(wavelength)
     y_min, y_max = 0, max(flux) + max(flux) * 0.05
 
     # create a polygon to define the top of the bars?
     polygon = Polygon(
-        np.vstack([
-            (x_min, 0),
-            tstack([wavelength[ok], flux[ok]]),
-            (x_max, 0),
-        ]),
-        facecolor='none',
-        edgecolor='none')
-    axes.add_patch(polygon)
+        np.vstack(
+            [
+                (x_min, 0),
+                tstack([wavelength[ok], flux[ok]]),
+                (x_max, 0),
+            ]
+        ),
+        facecolor="none",
+        edgecolor="none",
+    )
+    ax.add_patch(polygon)
 
     # draw bars, with the colors at each vertical stripe
     padding = 0.2
-    axes.bar(
-        x=wavelength[ok] - padding/2,
+    ax.bar(
+        x=wavelength[ok] - padding / 2,
         height=max(flux[ok]),
         width=1 + padding,
         color=colours,
-        align='edge')
+        align="edge",
+    )
 
-    # plot the actual spectrum?
-    # axes.plot(wavelength, values, color=COLOUR_STYLE_CONSTANTS.colour.dark)
+    return ax
 
-    return axes
 
-def rainbow_spectrum(axes=None,
-                 wavelength=None, flux=None,
-                 cmfs='CIE 1931 2 Degree Standard Observer',
-                 rainbowtop=np.inf,
-                 **kwargs):
+def plot_with_rainbow_fill(
+    ax=None,
+    wavelength=None,
+    flux=None,
+    cmfs="CIE 1931 2 Degree Standard Observer",
+    rainbowtop=np.inf,
+    **kwargs
+):
     """
     (This is still *real* blarg-y*.)
     Plot a spectrum, with a rainbow underneath.
 
     Parameters
     ----------
     ax : matplotlib.axes._subplots.AxesSubplot
@@ -120,64 +153,154 @@
 
     Returns
     -------
     ax : matplotlib.axes._subplots.AxesSubplot
         The ax into which the rainbow was drawn.
     """
 
-    if axes is None:
-        axes = plt.gca()
+    if ax is None:
+        ax = plt.gca()
 
     if wavelength is None:
         # create a grid of wavelengths (at which CMFss are useful)
         wavelength = CMFs.wavelengths
 
     # create y values that will be plotted (these could be spectrum)
     if flux is None:
         flux = np.ones_like(wavelength)
 
     # pull out only the values that *can* be converted to colors
-    ok = ((wavelength >= np.min(CMFs.wavelengths)) &
-          (wavelength <= np.max(CMFs.wavelengths)))
+    ok = (wavelength >= np.min(CMFs.wavelengths)) & (
+        wavelength <= np.max(CMFs.wavelengths)
+    )
 
     w, f = wavelength[ok], flux[ok]
 
     # clip the top of the box?
     f = np.minimum(f, rainbowtop)
 
     XYZ = wavelength_to_XYZ(w)
 
     # create colors at theose wavelengths
     colours = XYZ_to_plotting_colourspace(XYZ)
 
     # normalize the colors to their maximum?
-    #colours = COLOUR_STYLE_CONSTANTS.colour.colourspace.encoding_cctf(
+    # colours = CONSTANTS_COLOUR_STYLE.colour.colourspace.cctf_encoding(
     #    normalise_maximum(colours))
-    colours = np.maximum(0, colours/np.max(colours))
+    colours = np.maximum(0, colours / np.max(colours))
 
     x_min, x_max = min(w), max(w)
     y_min, y_max = 0, max(f) + max(f) * 0.05
 
     # create a polygon to define the top of the bars?
     polygon = Polygon(
-        np.vstack([
-            (x_min, 0),
-            tstack([w, f]),
-            (x_max, 0),
-        ]),
-        facecolor='none',
-        edgecolor='none')
-    axes.add_patch(polygon)
+        np.vstack(
+            [
+                (x_min, 0),
+                tstack([w, f]),
+                (x_max, 0),
+            ]
+        ),
+        facecolor="none",
+        edgecolor="none",
+    )
+    ax.add_patch(polygon)
 
     # draw bars, with the colors at each vertical stripe
     padding = 0.0
     dw = np.mean(np.diff(w))
-    axes.bar(
+    ax.bar(
         x=w,
         height=f,
         width=dw,
         color=colours,
         clip_path=polygon,
-        align='edge',
-        clip_on=True)
+        align="edge",
+        clip_on=True,
+    )
+
+    return ax
+
+
+def plot_as_slit_rainbow(
+    ax=None,
+    wavelength=None,
+    flux=None,
+    cmfs="CIE 1931 2 Degree Standard Observer",
+    **kwargs
+):
+    """
+    (This is still *real* blarg-y*.)
+    Plot a spectrum as a light source would be seen through
+    a slit spectrometer, with vertical bands of light that
+    are brighter or fainter depending on the intensity
+    of the spectrum at that particular wavelength.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes._subplots.AxesSubplot
+        The ax into which the rainbow should be drawn.
+
+    wavelength : array
+        The wavelengths to include in the spectrum.
+        In units of nm, but not as astropy units.
+
+    flux : array
+        The fluxes to include in the spectrum.
+        In units of whatever, but not as astropy units.
+
+    cmfs : string
+        The color matching function(s?) to use.
+
+    vector : bool
+
+
+    Returns
+    -------
+    ax : matplotlib.axes._subplots.AxesSubplot
+        The ax into which the rainbow was drawn.
+    """
+
+    # make sure our plotting ax is defined
+    if ax is None:
+        ax = plt.gca()
+
+    # make sure we have a grid of wavelengths defined
+    if wavelength is None:
+        # create a grid of wavelengths (at which CMFss are useful)
+        wavelength = CMFs.wavelengths
+
+    # create y values that will be plotted (these could be spectrum)
+    if flux is None:
+        flux = np.ones_like(wavelength)
+
+    # pull out only the values that *can* be converted to colors
+    ok = (wavelength >= np.min(CMFs.wavelengths)) & (
+        wavelength <= np.max(CMFs.wavelengths)
+    )
+    w, f = wavelength[ok], flux[ok]
+
+    # get the XYZ for the wavelengths
+    XYZ = wavelength_to_XYZ(w)
+
+    # create colors at those wavelengths
+    colours = XYZ_to_plotting_colourspace(XYZ)
+
+    # normalize the colors to their maximum?
+    # colours = CONSTANTS_COLOUR_STYLE.colour.colourspace.cctf_encoding(
+    #    normalise_maximum(colours))
+
+    # normalize the brightness by the flux
+    colours *= f[:, np.newaxis]
+
+    # normalize to the brightest line
+    colours = np.maximum(0, colours / np.max(colours))
+
+    # draw as an RGB color image with imshow
+    ax.imshow(
+        colours[np.newaxis, :, :],
+        aspect="auto",
+        extent=[np.min(w), np.max(w), 0, 1],
+        interpolation="nearest",
+    )
 
-    return axes
+    return ax
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/data/earthtransmission.txt` & `rainbow-connection-0.0.7/rainbowconnection/data/earthtransmission.txt`

 * *Files identical despite different names*

### Comparing `rainbow-connection-0.0.6/rainbowconnection/data/fortney/lambda_1500K_g10_noTiOVO.dat` & `rainbow-connection-0.0.7/rainbowconnection/data/fortney/lambda_1500K_g10_noTiOVO.dat`

 * *Files identical despite different names*

### Comparing `rainbow-connection-0.0.6/rainbowconnection/data/fortney/lambda_1500K_g10_wTiOVO.dat` & `rainbow-connection-0.0.7/rainbowconnection/data/fortney/lambda_1500K_g10_wTiOVO.dat`

 * *Files identical despite different names*

### Comparing `rainbow-connection-0.0.6/rainbowconnection/data/solarspectrum.txt` & `rainbow-connection-0.0.7/rainbowconnection/data/solarspectrum.txt`

 * *Files identical despite different names*

### Comparing `rainbow-connection-0.0.6/rainbowconnection/plottingtools.py` & `rainbow-connection-0.0.7/rainbowconnection/plottingtools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from .imports import *
-from .colortools import plot_rainbow
+from .colortools import plot_simple_rainbow
+
+
 def setup_axes_with_rainbow(ax=None, rainbow=True, figsize=(5, 2.5)):
     # create new ax(s), unless we're supposed to over plot on one
     if ax is None:
         plt.figure(figsize=figsize)
         # decide whether to add a horizontal rainbow cartoon
         if rainbow:
             # create a two-part grid
-            gs = GridSpec(  2, 1,
-                            height_ratios=[0.05, 1],
-                            hspace=0.0)
-
+            gs = GridSpec(2, 1, height_ratios=[0.05, 1], hspace=0.0)
 
             # plot a cartoon rainbow, in a box above
             ax_rainbow = plt.subplot(gs[0])
             plt.sca(ax_rainbow)
-            plot_rainbow(axes=ax_rainbow)
+            plot_simple_rainbow(ax=ax_rainbow)
 
             ax_rainbow.get_yaxis().set_visible(False)
             ax_rainbow.get_xaxis().set_visible(False)
-            ax_rainbow.set_facecolor('black')
+            ax_rainbow.set_facecolor("black")
             # (kludge to ensure black background for rainbow)
             if plt.gcf().get_facecolor() == (0.0, 0.0, 0.0, 1.0):
-                plt.axis('off')
+                plt.axis("off")
 
             # create the main ax
             ax = plt.subplot(gs[1], sharex=ax_rainbow)
 
         else:
             # simply create one simple ax
             ax = plt.subplot()
 
-
     # make sure we point back at the first plot
     plt.sca(ax)
     return ax
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/sources/Spectrum.py` & `rainbow-connection-0.0.7/rainbowconnection/sources/spectrum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from ..imports import *
-from ..colortools import plot_rainbow, rainbow_spectrum, CMFs, SpectralDistribution
+from ..colortools import (
+    plot_simple_rainbow,
+    plot_with_rainbow_fill,
+    plot_as_slit_rainbow,
+    CMFs,
+    SpectralDistribution,
+    ColourRuntimeWarning,
+)
 import colour
 from ..units import determine_quantity
 from ..plottingtools import setup_axes_with_rainbow
 
+
 def check_wavelength_unit(w):
-    w.to('micron')
+    w.to("micron")
+
+
+bgkw = dict(color="gray", alpha=0.5, zorder=-100)
 
-bgkw = dict(color='gray', alpha=0.5, zorder=-100)
 
 class Spectrum:
-    '''
+    """
     The Spectrum class is a generic representation of the light
     from some emitting object, particularly for spherically
     symmetric emission.
 
     By default, the `.spectrum(wavelength)` method will return
     the spectral luminosity of the object. This is a quantity
     with units like W/nm, and it can be integrated over
@@ -25,21 +35,21 @@
     the spectral flux from the object if seen from some
     particular distance. This is a quantity with units like
     W/nm/m**2, and it can be integrated over wavelength to
     provide the total flux of the light, in W/m**2.
 
     Classes that inherit from this will likely modify (at least)
     the surface_flux and surface_area methods.
-    '''
+    """
 
     # the default grid of wavelengths
-    default_wavelengths = np.arange(200, 1000)*u.nm
+    default_wavelengths = np.arange(200, 1000) * u.nm
 
-    def __init__(self, wavelength, flux, radius=1/4/np.pi*u.m):
-        '''
+    def __init__(self, wavelength, flux, radius=1 / 4 / np.pi * u.m):
+        """
         Initialize a spectrum by providing arrays of
         wavelength and flux. (Normally, some other
         wrapper will be used to create a new Spectrum
         object.)
 
         Parameters
         ----------
@@ -48,165 +58,166 @@
             These must be convertible to units of
             length (nm, m, cm, micron, Angstrom, ...)
 
         flux : astropy.units.quantity.Quantity
             The flux values of the spectrum. Units
             should be fairly flexible, but W/m**2/nm
             would be pretty reasonable defaults.
-        '''
+        """
 
         # make sure the wavelengths have some
         check_wavelength_unit(wavelength)
 
         # assign the hiddgen wavelength and flux values
         self._wavelength = wavelength
-        self._flux = flux*u.Unit('')
-        self.radius = radius*u.Unit('')
+        self._flux = flux * u.Unit("")
+        self.radius = radius * u.Unit("")
 
         # set the default wavelengths to be the actual values
         self.default_wavelengths = self._wavelength
 
     def surface_flux(self, wavelength=None):
 
         # make sure at least some grid of wavelengths is defined
         w = self.wavelength(wavelength)
 
         original_unit = self._flux.unit
         unitless_flux = self._flux.value
 
         # bin this spectrum to the particular wavelength grid
         unitless_neww, unitless_newf = bintogrid(
-            x=self._wavelength.to('nm').value,
+            x=self._wavelength.to("nm").value,
             y=unitless_flux,
-            newx=w.to('nm').value,
-            drop_nans=False)
+            newx=w.to("nm").value,
+            drop_nans=False,
+        )
 
         # make sure the wavelengths match up
-        assert(np.all(unitless_neww == w.to('nm').value))
+        assert np.all(unitless_neww == w.to("nm").value)
 
         # make sure the flux units match up
-        newf = unitless_newf*original_unit
-        assert(newf.unit.is_equivalent(self._flux.unit))
+        newf = unitless_newf * original_unit
+        assert newf.unit.is_equivalent(self._flux.unit)
 
         return newf
 
-
     def surface_area(self):
-        '''
+        """
         The surface area of the light source,
         in units like m**2.
 
         Returns
         -------
         surface_area : astropy.units.quantity.Quantity
             The emitting area of the surface, usually in m**2.
-        '''
-        return 4*np.pi*self.radius**2
-
+        """
+        return 4 * np.pi * self.radius ** 2
 
     def wavelength(self, wavelength=None):
-        '''
+        """
         A wrapper to ensure at least some grid of wavelengths
         gets defined. A default grid will be assumed, unless
         any wavelength array at all is passed.
-        '''
+        """
 
         # make sure at least some wavelengths are defined
         if wavelength is None:
             wavelength = self.default_wavelengths
-        return wavelength.to('nm')
+        return wavelength.to("nm")
 
     def spectrum(self, wavelength=None):
-        '''
+        """
         The spectrum of the light source, as spectral luminosity (W/nm)
         or if a distance is defined as spectral flux (W/nm/m**2).
 
         Parameters
         ----------
         wavelength : astropy.units.quantity.Quantity
             The wavelengths on which we want the spectrum.
 
         Returns
         -------
         spectrum : astropy.units.quantity.Quantity
             The luminosity (W/nm) or flux (W/nm/m**2).
-        '''
+        """
 
         # simplify the factor as best we can
-        factor = (self.surface_area()/self.normalization()).decompose()
+        factor = (self.surface_area() / self.normalization()).decompose()
 
         # return the surface flux with appropriate normalization
-        return factor*self.surface_flux(wavelength)
+        return factor * self.surface_flux(wavelength)
 
     def normalization(self):
-        '''
+        """
         The normalization by which this Spectrum
         will be divided. It's flexible, to allow
         either spectral luminosity or spectral flux.
 
         Returns
         -------
         norm : astropy.units.quantity.Quantity
             A normalization
-        '''
+        """
         try:
             # if there's a distance, return a flux
-            assert(self.distance is not None)
-            return 4*np.pi*self.distance**2
+            assert self.distance is not None
+            return 4 * np.pi * self.distance ** 2
         except (AttributeError, AssertionError):
             # by default, simply return a luminosity
             return 1.0
 
     def angular_size(self):
-        '''
+        """
         The angular size of the light source (if viewed from a distance).
-        '''
+        """
 
         try:
             # if there's a distance, return an angular size
-            assert(self.distance is not None)
-            return np.arctan(self.radius/self.distance).to('deg')
+            assert self.distance is not None
+            return np.arctan(self.radius / self.distance).to("deg")
         except (AttributeError, AssertionError):
             # complain if no distance is defined
-            raise ValueError('''
+            raise ValueError(
+                """
             This Spectrum has no .distance attribute.
             Please consider using `.at(distance)` to
             create a new light source as viewed from
             a distance.
-            ''')
+            """
+            )
 
-    def at(self, distance=1*u.au):
-        '''
+    def at(self, distance=1 * u.au):
+        """
         Create a new Spectrum representing the current
         light source viewed from some distance
         (assuming spherical symmetry).
 
         Parameters
         ----------
         distance : astropy.units.quantity.Quantity
             The distance at which we're viewing this source.
 
         Returns
         -------
         flux : Spectrum
             A new Spectrum, with the distance attached.
-        '''
+        """
 
         # create a copy of the current spectrum
         new = copy.deepcopy(self)
 
         # update this copy's distance and return
         new.distance = distance
         return new
 
     # FIXME -- for analytic functions, it'd help to define some kind of
     # a bounding box in wavelength space, so this integral could be done
     # analytically or with scipy.integrate.quad
     def integrate(self, lower=None, upper=None):
-        '''
+        """
         Integrate the spectrum over wavelength.
 
         It gives a number with units identical to the results of
         `.spectrum()` but without the wavelength (W or W/m**2).
 
         Parameters
         ----------
@@ -216,207 +227,207 @@
         upper : astropy.units.quantity.Quantity
             The lower wavelength limit.
 
         Returns
         -------
         integral : astropy.units.quantity.Quantity
             The integral over wavelength
-        '''
+        """
 
         w = self.default_wavelengths
         f = self.spectrum(w)
 
-
-        ok = np.ones(np.shape(w)).astype(np.bool)
+        ok = np.ones(np.shape(w)).astype(bool)
         if lower is not None:
             ok *= w >= lower
 
         if upper is not None:
             ok *= w <= upper
-            #raise NotImplementedError('Wavelength limits not yet OK.')
-
+            # raise NotImplementedError('Wavelength limits not yet OK.')
 
         return np.trapz(f[ok], w[ok])
 
-        #np.trapz(f.value, w.value)*f.unit*w.unit
-        #wlower = lower or self.default_wavelengths[0]
-        #wupper = upper or self.default_wavelengths[-1]
-        #return quad(self.spectrum, wlower, wupper)
-
-
+        # np.trapz(f.value, w.value)*f.unit*w.unit
+        # wlower = lower or self.default_wavelengths[0]
+        # wupper = upper or self.default_wavelengths[-1]
+        # return quad(self.spectrum, wlower, wupper)
 
     def to_sd(self):
-        '''
+        """
         Create a `colour` SpectralDistribution from this object,
         solely covering the visible range. This can be used
         to estimate the true color of this spectrum.
-        '''
+        """
 
         # pick wavelengths directly from the color-matching functions
-        w = CMFs.wavelengths*u.nm
+        w = CMFs.wavelengths * u.nm
 
         # normalize only within the visible range
-        ok = (w < 700*u.nm) & (w > 390*u.nm)
+        ok = (w < 700 * u.nm) & (w > 390 * u.nm)
         w = w[ok]
         # (note: this is a kludge to avoid making spectra
         #  with most of their luminosity outside the visible
         #  appear as really dark and dull. there is probably
         #  a much cleverer way of making sure the normalization
         #  does something reasonable.)
 
         # calculate the spectrum at those wavelengths
         f = self.spectrum(w)
 
         # create the spectral distribution
-        sd = SpectralDistribution(dict(zip(w.value, f.value/np.max(f.value))))
+        sd = SpectralDistribution(dict(zip(w.value, f.value / np.max(f.value))))
 
         # return it
         return sd
 
     def to_color(self):
-        '''
+        """
         Determine the RGB color of this spectrum.
 
         Returns
         -------
         rgb : numpy.ndarray
             3-element array containing RGB values
             that can be fed into matplotlib.
-        '''
+        """
 
-        # create a colour SpectralDistribution
-        sd = self.to_sd()
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore", category=ColourRuntimeWarning)
 
-        # convert to XYZ
-        # (maybe use `k=` option for relative scaling between sources?)
-        XYZ = colour.sd_to_XYZ(sd)
-        if (np.min(XYZ) < 0) or np.max(XYZ) > 100:
-            print(f'XYZ={XYZ} is outside of [0, 100]!')
-
-        # convert to RGB
-        RGB = colour.XYZ_to_sRGB(XYZ / 100)
-        if (np.min(RGB) < 0) or np.max(RGB) > 1:
-            pass
-            #print(f'RGB={RGB} is outside of [0, 1]!')
-
-        # trim out underenderable colors (this is sneaky!)
-        #clipped_RGB = np.maximum(0, np.minimum(1, RGB))
-        clipped_RGB = np.maximum(0, RGB)
-        # instead of clip, should we add to everything until we get to zero?
-
-        # kludge to maximize brightness, for every color!
-        clipped_RGB /= np.max(clipped_RGB)
-        return clipped_RGB
+            # create a colour SpectralDistribution
+            sd = self.to_sd()
+
+            # convert to XYZ
+            # (maybe use `k=` option for relative scaling between sources?)
+            XYZ = colour.sd_to_XYZ(sd)
+            if (np.min(XYZ) < 0) or np.max(XYZ) > 100:
+                print(f"XYZ={XYZ} is outside of [0, 100]!")
+
+            # convert to RGB
+            RGB = colour.XYZ_to_sRGB(XYZ / 100)
+            if (np.min(RGB) < 0) or np.max(RGB) > 1:
+                pass
+                # print(f'RGB={RGB} is outside of [0, 1]!')
+
+            # trim out underenderable colors (this is sneaky!)
+            # clipped_RGB = np.maximum(0, np.minimum(1, RGB))
+            clipped_RGB = np.maximum(0, RGB)
+            # instead of clip, should we add to everything until we get to zero?
+
+            # kludge to maximize brightness, for every color!
+            clipped_RGB /= np.max(clipped_RGB)
+            return clipped_RGB
 
     def __repr__(self):
-        '''
+        """
         How should this object appear as a string?
 
         Returns
         -------
         s : str
             A simple string representation.
-        '''
+        """
         try:
-            assert(self.distance is not None)
-            return f'{self.__class__.__name__} at {self.distance}'
+            assert self.distance is not None
+            return f"{self.__class__.__name__} at {self.distance}"
         except (AssertionError, AttributeError):
-            return f'{self.__class__.__name__}'
+            return f"{self.__class__.__name__}"
 
-    def set_power(self, power=100*u.W):
-        '''
+    def set_power(self, power=100 * u.W):
+        """
         Change the radius of the object so that it will
         emit a specified power, with the same spectral shape.
 
         Parameters
         ----------
         power : astropy.units.quantity.Quantity
             The total power we want the object to emit.
-        '''
+        """
 
         # calculate the total luminosity of this object
         total = self.integrate()
 
         # make sure we're dealing with an actual luminosity
-        assert(total.unit.is_equivalent('W'))
+        assert total.unit.is_equivalent("W")
 
         # calculation a new normalization
-        normalization = (power/total).decompose()
+        normalization = (power / total).decompose()
 
         # change the radius of this object
         self.radius *= np.sqrt(normalization)
         self.power = power
 
     def mean_intensity(self, wavelength=None):
-        '''
+        """
         Calculate the mean intensity field created by the source.
 
         The mean intensity field represents the intensity
         of the source, smeared over a full 4pi steradians.
 
         (This makes sense only for spectra viewed from a distance.)
-        '''
+        """
 
         # what is the intensity of the disk
         F_disk = self.spectrum(wavelength)
 
-
         # make sure we're dealing with a flux
-        assert(F_disk.unit.is_equivalent(u.W/u.m**2/u.nm))
+        assert F_disk.unit.is_equivalent(u.W / u.m ** 2 / u.nm)
 
         # calculate the mean intensity
-        solid_angle = np.pi*self.angular_size()**2
+        solid_angle = np.pi * self.angular_size() ** 2
 
         # calculate the mean intensity field
-        J = F_disk/4/np.pi/u.sr
+        J = F_disk / 4 / np.pi / u.sr
 
         return J
 
     def disk_intensity(self, wavelength=None):
-        '''
+        """
         Calculate the intensity of the disk of the source.
 
         The disk intensity represents the intensity of staring
         directly at the disk. The flux of the source is its
         intensity integrated over solid angle, so two sources
         with the same intensities can have very different
         fluxes, based on their apparent angular sizes.
         For example, the Sun seen `.at` different distances
         will have different fluxes but the same disk intensity.
 
         (This makes sense only for spectra viewed from a distance.)
-        '''
+        """
 
         # what is the intensity of the disk
         F_disk = self.spectrum(wavelength)
 
-
         # make sure we're dealing with a flux
-        assert(F_disk.unit.is_equivalent(u.W/u.m**2/u.nm))
+        assert F_disk.unit.is_equivalent(u.W / u.m ** 2 / u.nm)
 
         # calculate the mean intensity
-        solid_angle = np.pi*self.angular_size()**2
-        I_disk = F_disk/solid_angle
+        solid_angle = np.pi * self.angular_size() ** 2
+        I_disk = F_disk / solid_angle
 
         return I_disk
 
     # ===================================
     #
     #        PLOTTING METHODS
     #
     # ===================================
 
-    def plot(self,  ax=None,
-                    wavelength=None,
-                    rainbow=True,
-                    color='auto',
-                    style='dark_background',
-                    figsize=(5, 2.5),
-                    **kwargs):
-        '''
+    def plot(
+        self,
+        ax=None,
+        wavelength=None,
+        rainbow=True,
+        color="auto",
+        style="dark_background",
+        figsize=(5, 2.5),
+        **kwargs,
+    ):
+        """
         A quick tool to plot a spectrum.
 
         Parameters
         ----------
         ax : matplotlib.axes._subplots.AxesSubplot
             Specify an axes object into which
             this plot should be drawn. This allows
@@ -437,57 +448,61 @@
             Should we add an extra rainbow above the plot,
             to indicate how wavelengths match to visible light?
 
         color : str
             The color for drawing the spectrum.
             'auto' represents the actual visible color.
 
-        '''
+        """
 
         # set up to use a dark background for the plot; make sure units match
         with plt.style.context(style), quantity_support():
 
             # setup the basic axes
             ax = setup_axes_with_rainbow(ax=ax, rainbow=rainbow, figsize=figsize)
 
             # make sure at least some wavelengths are defined
             w = self.wavelength(wavelength)
 
             # pull out the spectrum
             f = self.spectrum(w)
 
             # plot the spectrum
-            if color == 'auto':
+            if color == "auto":
                 color = self.to_color()
                 background = ax.get_facecolor()[0:3]
                 if np.max(color - background) < 0.05:
-                    print(f'''
+                    print(
+                        f"""
                     The inferred color {color} might be a little
                     too close to {background} to be visible. Consider
                     plotting without the `color='auto'` option.
-                    ''')
+                    """
+                    )
             plt.plot(w, f, color=color, label=self, **kwargs)
 
             # add the axis labels
-            wunit = w.unit.to_string('latex_inline')
-            funit = f.unit.to_string('latex_inline')
-            plt.xlabel(f'Wavelength ({wunit})')
-            plt.ylabel(f'{determine_quantity(f.unit)} ({funit})')
+            wunit = w.unit.to_string("latex_inline")
+            funit = f.unit.to_string("latex_inline")
+            plt.xlabel(f"Wavelength ({wunit})")
+            plt.ylabel(f"{determine_quantity(f.unit)} ({funit})")
 
         return ax
 
-
-    def plot_rgb(self,  ax=None,
-                        wavelength=None,
-                        rainbow=True,
-                        foreground=True,
-                        style='dark_background',
-                        figsize=(5, 2.5),
-                        **kwargs):
-        '''
+    def plot_rgb(
+        self,
+        ax=None,
+        wavelength=None,
+        rainbow=True,
+        foreground=True,
+        style="dark_background",
+        figsize=(5, 2.5),
+        **kwargs,
+    ):
+        """
         A quick tool to plot a spectrum, just as RGB bars.
 
         Parameters
         ----------
         ax : matplotlib.axes._subplots.AxesSubplot
             Specify an axes object into which
             this plot should be drawn. This allows
@@ -508,15 +523,15 @@
             Should we add an extra rainbow above the plot,
             to indicate how wavelengths match to visible light?
 
         color : str
             The color for drawing the spectrum.
             'auto' represents the actual visible color.
 
-        '''
+        """
 
         # set up to use a dark background for the plot; make sure units match
         with plt.style.context(style), quantity_support():
 
             # setup the basic axes
             ax = setup_axes_with_rainbow(ax=ax, rainbow=rainbow, figsize=figsize)
 
@@ -529,43 +544,55 @@
             green = [495, 590]
             red = [590, 685]
 
             centers = [np.mean(c) for c in [red, green, blue]]
             widths = [c[1] - c[0] for c in [red, green, blue]]
 
             if foreground:
-                kw = dict(color = [np.array([1, 0, 0]),
-                                   np.array([0, 1, 0]),
-                                   np.array([0, 0, 1])],
-                          edgecolor='white',
-                          zorder = 0)
+                kw = dict(
+                    color=[
+                        np.array([1, 0, 0]),
+                        np.array([0, 1, 0]),
+                        np.array([0, 0, 1]),
+                    ],
+                    edgecolor="white",
+                    zorder=0,
+                )
             else:
 
                 kw = dict(**bgkw)
-                kw['edgecolor'] = 'none'
-            plt.bar(centers, rgb*100, widths, **kw) # linewidth=2,
-
+                kw["edgecolor"] = "none"
+            plt.bar(centers, rgb * 100, widths, **kw)  # linewidth=2,
 
             # add the axis labels
-            wunit = w.unit.to_string('latex_inline')
-            plt.xlabel(f'Wavelength ({wunit})')
-            plt.ylabel(f'Brightness (%)')
+            wunit = w.unit.to_string("latex_inline")
+            plt.xlabel(f"Wavelength ({wunit})")
+            plt.ylabel(f"Brightness (%)")
 
         return ax
 
-    def plot_as_rainbow(self,  ax=None,
-                                rainbow=True,
-                                color='auto',
-                                style='dark_background',
-                                foreground=True,
-                                ylim=[0, 120],
-                                figsize=(5,2.5),
-                                **kwargs):
-        '''
-        A quick tool to plot a spectrum, just as RGB bars.
+    def plot_as_rainbow(
+        self,
+        ax=None,
+        rainbow=True,
+        color="auto",
+        style="dark_background",
+        foreground=True,
+        ylim=[0, 120],
+        figsize=(5, 2.5),
+        **kwargs,
+    ):
+        """
+        A quick tool to plot a spectrum with the height
+        as the flux, and a continuous rainbow filling
+        in undernearth it.
+
+        The relative amount of light at different wavelengths
+        will be represented by the different area taken up
+        by colored pixels at that wavelength.
 
         Parameters
         ----------
         ax : matplotlib.axes._subplots.AxesSubplot
             Specify an axes object into which
             this plot should be drawn. This allows
             overplotting multiple spectra, for example
@@ -585,51 +612,123 @@
             Should we add an extra rainbow above the plot,
             to indicate how wavelengths match to visible light?
 
         color : str
             The color for drawing the spectrum.
             'auto' represents the actual visible color.
 
-        '''
+        """
 
         # set up to use a dark background for the plot; make sure units match
         with plt.style.context(style), quantity_support():
 
             # setup the basic axes
             ax = setup_axes_with_rainbow(ax=ax, rainbow=rainbow, figsize=figsize)
 
             # make sure at least some wavelengths are defined
-            w = self.wavelength(np.arange(330, 760, 1)*u.nm)
+            w = self.wavelength(np.arange(330, 760, 1) * u.nm)
             f = self.spectrum(w)
             # KLUDGE?
-            norm = np.max(f.value[(w > 400*u.nm) & (w < 685*u.nm)]) / 100
+            norm = np.max(f.value[(w > 400 * u.nm) & (w < 685 * u.nm)]) / 100
             if foreground:
-                rainbow_spectrum(axes=ax, wavelength=w.to('nm').value, flux=f.value/norm,
-                                 rainbowtop=np.max(ylim))
-                plt.plot(w, f/norm, color='white') #, linewidth=2
+                plot_with_rainbow_fill(
+                    ax=ax,
+                    wavelength=w.to("nm").value,
+                    flux=f.value / norm,
+                    rainbowtop=np.max(ylim),
+                )
+                plt.plot(w, f / norm, color="white")  # , linewidth=2
             else:
-                plt.fill_between(w, f/norm, linewidth=0, **bgkw)
+                plt.fill_between(w, f / norm, linewidth=0, **bgkw)
             plt.ylim(*ylim)
 
             # add the axis labels
-            wunit = w.unit.to_string('latex_inline')
-            plt.xlabel(f'Wavelength ({wunit})')
-            plt.ylabel(f'Brightness (%)')
+            wunit = w.unit.to_string("latex_inline")
+            plt.xlabel(f"Wavelength ({wunit})")
+            plt.ylabel(f"Brightness (%)")
+
+        return ax
+
+    def plot_as_slit_rainbow(
+        self,
+        ax=None,
+        rainbow=True,
+        style="dark_background",
+        figsize=(5, 2.5),
+        xlim=[360 * u.nm, 760 * u.nm],
+        dw=1 * u.nm,
+        **kwargs,
+    ):
+        """
+        A quick tool to plot a spectrum as it would appear
+        through a slit spectrometer. The relative amount of
+        light at different wavelengths will be represented
+        by the brightness of bars at those wavelengths.
+
+        Parameters
+        ----------
+        ax : matplotlib.axes._subplots.AxesSubplot
+            Specify an axes object into which
+            this plot should be drawn. This allows
+            overplotting multiple spectra, for example
+            with a structure like
+                ```
+                ax = Thermal(teff=5800*u.K, radius=1*u.Rsun).plot()
+                ax = Sun.plot(ax)
+                ```
+            To overplot on current axes use `ax=plt.gca()`.
+
+        wavelength : astropy.units.quantity.Quantity
+            A grid of wavelengths on which the spectrum should
+            be plotted. If None, the function defaults to
+            covering visible wavelengths at 1nm resolution.
+
+        rainbow : bool
+            Should we add an extra rainbow above the plot,
+            to indicate how wavelengths match to visible light?
+        """
+
+        # set up to use a dark background for the plot; make sure units match
+        with plt.style.context(style), quantity_support():
+
+            # setup the basic axes
+            ax = setup_axes_with_rainbow(ax=ax, rainbow=rainbow, figsize=figsize)
+
+            # make sure at least some wavelengths are defined
+
+            w = self.wavelength(
+                np.arange(
+                    xlim[0].to("nm").value, xlim[1].to("nm").value, dw.to("nm").value
+                )
+                * u.nm
+            )
+            f = self.spectrum(w)
+
+            plot_as_slit_rainbow(
+                ax=ax, wavelength=w.to("nm").value, flux=f.value, **kwargs
+            )
+
+            # add the axis labels
+            wunit = w.unit.to_string("latex_inline")
+            plt.xlabel(f"Wavelength ({wunit})")
+
+            plt.ylim(0, 1)
+            plt.xlim(*xlim)
 
         return ax
 
     def cartoon_sun(self):
-        '''
+        """
         Create a simple cartoon of the star,
         with appropriate color and angular size.
-        '''
+        """
 
         # figure out the color of the star
         rgb = self.to_color()
 
-        with plt.style.context('dark_background'):
+        with plt.style.context("dark_background"):
             fi = plt.figure(figsize=(5, 2.5))
             ax = fi.add_axes([0, 0, 1, 1])
             plt.scatter(0, 0, c=rgb, s=8000)
             plt.xticks([])
             plt.yticks([])
-            plt.axis('off')
+            plt.axis("off")
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/sources/Thermal.py` & `rainbow-connection-0.0.7/rainbowconnection/sources/thermal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 from .spectrum import *
 
+
 class Thermal(Spectrum):
-    def __init__(self, teff=5800*u.K, radius=1*u.Rsun):
+    def __init__(self, teff=5800 * u.K, radius=1 * u.Rsun):
 
         self.teff = teff
         self.radius = radius
 
     def intensity(self, wavelength):
-        '''
+        """
         This function calculates the thermal emission intensity spectrum of a surface.
 
             Inputs:
                 wavelength = numpy array of wavelengths (with astropy units)
 
             Outputs:
                 Returns an array of thermal emission intensities,
                 in astropy units of W/(m^2*micron*sr). This is a flux, which has
                 already been integrated over solid angle.
-        '''
+        """
 
         temperature = self.teff
 
         # define variables as shortcut to the constants we need
         h = con.h
         k = con.k_B
         c = con.c
 
         # this is the thing that goes into the exponent (it's units better cancel!)
-        up = h*c/(wavelength*k*temperature)
+        up = h * c / (wavelength * k * temperature)
 
         # calculate the intensity from the Planck function
-        intensity = (2*h*c**2/wavelength**5/(np.exp(up) - 1))/u.steradian
+        intensity = (2 * h * c ** 2 / wavelength ** 5 / (np.exp(up) - 1)) / u.steradian
 
         # return the intensity
-        return intensity.to('W/(m**2*nm*sr)')
+        return intensity.to("W/(m**2*nm*sr)")
 
     def surface_flux(self, wavelength):
-        '''
+        """
         This function calculates the thermal emission flux spectrum of a surface.
 
             Inputs:
                 wavelength = numpy array of wavelengths (with astropy units)
                 temperature = a single number, the temperature (with astropy units)
 
             Outputs:
                 Returns an array of thermal emission fluxes,
                 in astropy units of W/(m^2*micron). This is a flux, which has
                 already been integrated over solid angle.
-        '''
+        """
 
         # calculate the flux, knowing the angle integral will be pi steradians (for isotropic emission)
-        flux = self.intensity(wavelength)*np.pi*u.steradian
+        flux = self.intensity(wavelength) * np.pi * u.steradian
 
         # return the flux, in convenient units
-        return flux.to('W/(nm * m**2)')
+        return flux.to("W/(nm * m**2)")
 
     def __repr__(self):
-        '''
+        """
         How should this object appear as a string?
 
         Returns
         -------
         s : str
             A simple string representation.
-        '''
+        """
 
-        basic = f'{self.__class__.__name__} ({self.teff:.0f}, {self.radius})'
+        basic = f"{self.__class__.__name__} ({self.teff:.0f}, {self.radius})"
         try:
-            assert(self.distance is not None)
-            return basic + f' at {self.distance}'
+            assert self.distance is not None
+            return basic + f" at {self.distance}"
         except (AssertionError, AttributeError):
             return basic
 
     def integrate(self, lower=None, upper=None):
-        '''
+        """
         Integrate the spectrum over wavelength.
 
         It gives a number with units identical to the results of
         `.spectrum()` but without the wavelength (W or W/m**2).
 
         Parameters
         ----------
@@ -87,17 +88,17 @@
         upper : astropy.units.quantity.Quantity
             The lower wavelength limit.
 
         Returns
         -------
         integral : astropy.units.quantity.Quantity
             The integral over wavelength.
-        '''
+        """
 
         # if wavelength limits are used, revert back to the numerical integral
         if (lower is not None) or (upper is not None):
             return super().integrate(lower=lower, upper=upper)
 
         # if there are infinite wavelength limits, do the integral analytically
-        surface_flux = con.sigma_sb*self.teff**4
-        factor = (self.surface_area()/self.normalization()).decompose()
-        return factor*surface_flux
+        surface_flux = con.sigma_sb * self.teff ** 4
+        factor = (self.surface_area() / self.normalization()).decompose()
+        return factor * surface_flux
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/library.py` & `rainbow-connection-0.0.7/rainbowconnection/sources/phoenix/library.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,271 +1,376 @@
-'''
+"""
 Set up what's needed to access a directory full
 of PHOENIX model spectra.
-'''
+"""
 
-__all__ = ['get_metallicity_directory', 'unzip_metallicity', 'setup_metallicities', 'read_exact_phoenix', 'read_phoenix']
+__all__ = [
+    "get_metallicity_directory",
+    "unzip_metallicity",
+    "setup_metallicities",
+    "read_exact_phoenix",
+    "read_phoenix",
+]
 
 from ...imports import *
 from .utils import *
 from ...resampletools import *
-
-from craftroom.utils import find_nearest, find_two_nearest, interpolation_weights
 from astropy.io import fits
+from ..thermal import Thermal
 
 preloaded = {}
 
 # specify where to get the data from online
-base_url = 'http://phoenix.astro.physik.uni-goettingen.de/data/'
-online_library_directory = 'MedResFITS/R10000FITS/'
+base_url = "http://phoenix.astro.physik.uni-goettingen.de/data/"
+online_library_directory = "MedResFITS/R10000FITS/"
 
 # FIXME -- make the local storage directory more flexible?
-base_directory = os.path.join(os.getenv('HOME'), '.rainbow-connection')
-directory_template = 'PHOENIX-ACES-AGSS-COND-2011_R10000FITS_Z{metallicity}'
+base_directory = os.path.join(os.getenv("HOME"), ".rainbow-connection")
+directory_template = "PHOENIX-ACES-AGSS-COND-2011_R10000FITS_Z{metallicity}"
 
 # define a more flexible template string to catch all files
-file_template = 'lte{Teff:05.0f}-{logg:04.2f}{metallicity}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits'
-flexible_file_template = 'lte*-*{metallicity}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits'
+file_template = (
+    "lte{Teff:05.0f}-{logg:04.2f}{metallicity}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits"
+)
+flexible_file_template = "lte*-*{metallicity}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits"
 
 
 def get_metallicity_directory(Z=0.0):
-    '''
+    """
     Figure out model directory for a particular metallicity.
 
     Parameters
     ----------
     Z : float
         [Fe/H]-style metallicity (= 0.0 for solar)
-    '''
+    """
     return directory_template.format(metallicity=stringify_metallicity(Z))
 
+
 def get_metallicity_url(Z=0.0):
-    '''
+    """
     Figure out the URL to download a particular
     metallicity subset of models.
 
     Parameters
     ----------
     Z : float
         [Fe/H]-style metallicity (= 0.0 for solar)
-    '''
+    """
     model_directory = get_metallicity_directory(Z)
-    url = f'{base_url}{online_library_directory}{model_directory}.zip'
+    url = f"{base_url}{online_library_directory}{model_directory}.zip"
     return url
 
+
 def download_metallicity(Z=0.0):
-    '''
+    """
     Make sure the zip file of a particular metallicity has
     been downloaded.
 
     Parameters
     ----------
     Z : float
         [Fe/H]-style metallicity (= 0.0 for solar)
-    '''
+    """
 
     # what's the URL of the file to download
     url = get_metallicity_url(Z)
 
-    print(f'''
+    print(
+        f"""
     Checking for a cached version of
     {url}
     or downloading it for the first time.
-    ''')
-    filename = download_file(url,
-                             cache=True,
-                             show_progress=True,
-                             pkgname=package_name)
+    """
+    )
+    filename = download_file(url, cache=True, show_progress=True, pkgname=package_name)
 
     return filename
 
+
 def unzip_metallicity(Z=0.0):
-    '''
+    """
     Unzip the downloaded PHOENIX model zip file.
     (Figure out the URL from the metallicity,
     make sure astropy has downloaded it into the
     cache directory, and then unzip into a more
     friendly directory structure.)
 
     Parameters
     ----------
     Z : float
         [Fe/H]-style metallicity (= 0.0 for solar)
-    '''
+    """
 
     # figure out the local
     url = get_metallicity_url(Z)
     local_path_to_zip_file = download_metallicity(Z)
 
     # find the base directory (something like /Users/zkbt/.rainbow-connection/)
-    i_base = local_path_to_zip_file.find('cache/download')
-    assert(i_base > 0)
+    i_base = local_path_to_zip_file.find("cache/download")
+    assert i_base > 0
     local_base_directory = local_path_to_zip_file[:i_base]
-    local_directory = os.path.join(local_base_directory,
-                                   get_metallicity_directory(Z))
+    local_directory = os.path.join(local_base_directory, get_metallicity_directory(Z))
 
     # check if unzipped files already exist
-    pattern = os.path.join(local_directory, '*.fits')
+    pattern = os.path.join(local_directory, "*.fits")
     unzipped_files = glob.glob(pattern)
     N = len(unzipped_files)
-    print(f'''
+    print(
+        f"""
     Checking the file pattern
     {pattern}
     for existing models that have already been extracted.
-    ''')
+    """
+    )
     if N > 0:
-        print(f'''
+        print(
+            f"""
     The file pattern
     {pattern}
     already matches {N} files.
     If you want to re-extract these files,
     please delete the existing ones.
-        ''')
+        """
+        )
     else:
         # update what's happening
-        print(f'''
+        print(
+            f"""
         The file downloaded from
         {url}
         was stored locally as
         {local_path_to_zip_file}
         and is now being unzipped to
         {local_directory}
         It may take a while...
-        ''')
-        with zipfile.ZipFile(local_path_to_zip_file, 'r') as zip_ref:
+        """
+        )
+        with zipfile.ZipFile(local_path_to_zip_file, "r") as zip_ref:
             zip_ref.extractall(local_directory)
 
     return local_directory
 
+
 def setup_metallicities(Zs=[-0.5, 0.0, 0.5]):
-    '''
+    """
     Download and unzip a set of metallicities.
 
     Parameters
     ----------
     Z : list, array
         [Fe/H]-style metallicities (= 0.0 for solar)
-    '''
+    """
     for Z in Zs:
         unzip_metallicity(Z)
 
+
 def get_downloaded_models():
-    '''
+    """
     Identify what models have already been downloaded,
     in terms of metallicity, Teff, logg.
 
     Returns
     -------
     available : dict
         A dictionary with (float) metallicities as keys.
         Each value is a pair of arrays (Teff, logg) to
         indicate the values of effective temperature and
         log(surface gravity) that are available for that
         surface gravity value.
-    '''
+    """
 
     # figure out what metallicity directories are avaialble
-    available_metallicity_directories = glob.glob(os.path.join(base_directory,
-                                                               directory_template.format(metallicity='*')))
-
-    available_metallicities = {float(d.split('/')[-1].split('_Z')[-1]):d
-                               for d in available_metallicity_directories}
+    available_metallicity_directories = glob.glob(
+        os.path.join(
+            base_directory,
+            directory_template.format(metallicity="*"),
+        )
+    )
+
+    available_metallicities = {
+        float(d.split("/")[-1].split("_Z")[-1]): d
+        for d in available_metallicity_directories
+    }
 
     availability_by_metallicity = {}
-    print(available_metallicities)
-    for metallicity in available_metallicities:
-        Z = stringify_metallicity(metallicity)
-        this_metallicity = os.path.join(base_directory,
-                                        directory_template,
-                                        flexible_file_template).format(metallicity=stringify_metallicity(metallicity))
-
-        # for now, just interpolate in temperature
-        Teffs, loggs = [], []
-        for t in np.sort(glob.glob(this_metallicity)):
-            x = (t.split('/lte')[-1].split('-')[0:2])
-            Teffs.append(np.float(x[0]))
-            loggs.append(np.float(x[1].split('+')[0]))
-        Teffs = np.array(Teffs)
-        loggs = np.array(loggs)
 
-
-        availability_by_metallicity[metallicity] = Teffs, loggs
-        print('[Fe/H] = {} has {} spectra'.format(metallicity, len(Teffs)))
+    if len(available_metallicities) == 0:
+        print(
+            """
+        It is totally fine to proceed using `rainbow-connection` as is, without
+        downloading any addition files. However, if you want to have access
+        access to stellar spectra of arbitrary temperatures, you will need
+        to download some PHOENIX model spectra to your computer. It appears
+        that no spectra have yet been downloaded.
+
+        To download a set of model spectra for a particular metallicity, run
+        ```
+        from rainbowconnection.sources.phoenix import unzip_metallicity
+        unzip_metallicity(Z=0.0)
+        ```
+        replacing the `Z=` argument with whatever (log-solar) metallicity
+        you want to download. Available options are in increments of 0.5 dex.
+
+        This will download a very large file for each metallicty, so it may
+        take a fairly long time. Please be patient. It will download and
+        unzip these files into a (hidden) directory called `.rainbow-connection`
+        in your $HOME directory.
+        """
+        )
+    else:
+        print(
+            "The following PHOENIX stellar spectra have been downloaded\n"
+            "and are available to use via `Star()` source objects:\n"
+        )
+        for metallicity in available_metallicities:
+            Z = stringify_metallicity(metallicity)
+            this_metallicity = os.path.join(
+                base_directory,
+                directory_template,
+                flexible_file_template,
+            ).format(metallicity=stringify_metallicity(metallicity))
+
+            # for now, just interpolate in temperature
+            Teffs, loggs = [], []
+            for t in np.sort(glob.glob(this_metallicity)):
+                x = t.split("/lte")[-1].split("-")[0:2]
+                Teffs.append(float(x[0]))
+                loggs.append(float(x[1].split("+")[0]))
+            Teffs = np.array(Teffs)
+            loggs = np.array(loggs)
+
+            availability_by_metallicity[metallicity] = (
+                Teffs,
+                loggs,
+            )
+            print(
+                f"Metallicity [Fe/H] = {metallicity} has {len(Teffs)} spectra, stored in..."
+            )
+            print(f" {this_metallicity}")
 
     return availability_by_metallicity
 
 
 availability_by_metallicity = get_downloaded_models()
 
-def read_exact_phoenix(Teff=5800, logg=4.5, metallicity=0.0, photons=True, R=None):
+
+def read_exact_phoenix(Teff=5800, logg=4.5, metallicity=0.0, photons=True, R=None, extend_wavelengths=False):
 
     key = (Teff, logg, metallicity, photons, R)
 
     try:
         wave, flux = preloaded[key]
     except KeyError:
-        filename = os.path.join(base_directory, directory_template, file_template).format(Teff=Teff, logg=logg, metallicity=stringify_metallicity(metallicity))
+        filename = os.path.join(
+            base_directory, directory_template, file_template
+        ).format(
+            Teff=Teff,
+            logg=logg,
+            metallicity=stringify_metallicity(metallicity),
+        )
 
         hdus = fits.open(filename)
         # flux units are erg/s/cm^2/cm
         flux_cgs = hdus[0].data
         # flux units are erg/s/cm^2/nm
-        flux_nm = flux_cgs/1e7
-        h = hdus[0].header
+        flux_nm = flux_cgs / 1e7
+        header = hdus[0].header
 
         # wavelength units are nm
-        wave = np.exp(h['CRVAL1'] + h['CDELT1']*np.arange(h['NAXIS1']))/10
-
-        '''
-        # include kludge to extend to wavelengths beyond 2500nm
-        t = rc.Thermal(Teff*u.K, radius=1*u.Rsun).at(1*u.Rsun)
-        extra_wave = np.linspace(np.max(wave) + 100, 6000)*u.nm
-        extra_flux = t.surface_flux(extra_wave).to('erg/(s * cm**2 * nm)')
-
-        wave = np.hstack([wave, extra_wave.value])
-        flux_nm = np.hstack([flux_nm, extra_flux.value])
-        '''
-
-        #energy = (con.h*con.c/w/u.ph).to('J/ph')
-        #f = (t.surface_flux(w)/energy).to('ph/(s * cm**2 * nm)')
-
+        wave = np.exp(header["CRVAL1"] + header["CDELT1"] * np.arange(header["NAXIS1"])) / 10
 
+        if extend_wavelengths:
+            # include kludge to extend to wavelengths beyond 2500nm
+            t = Thermal(Teff*u.K, radius=1*u.Rsun).at(1*u.Rsun)
+            extra_wave = np.linspace(np.max(wave), 6000)*u.nm
+            extra_flux = t.surface_flux(extra_wave).to('erg/(s * cm**2 * nm)')
+
+            wave = np.hstack([wave, extra_wave.value])
+            flux_nm = np.hstack([flux_nm, extra_flux.value])
+
+        # energy = (con.h*con.c/w/u.ph).to('J/ph')
+        # f = (t.surface_flux(w)/energy).to('ph/(s * cm**2 * nm)')
+        """
+        k_B = 1.38e-16       # erg/K
+        if extend_wavelengths:
+
+            # define extra wavelength grid
+            original_R = 1/header["CDELT1"]
+            w_extra = np.max(wave)*np.exp(np.arange(int(original_R))/original_R)
+            w_extra_in_cm = w_extra/1e7
+
+            # calculate the thing in the
+            up = h * c / (w_extra_in_cm * k_B * Teff)
+
+            # calculate the intensity from the Planck function
+            flux_extra = np.pi * (2 * h * c ** 2 / w_extra_in_cm ** 5 / (np.exp(up) - 1))
+
+            wave = np.hstack([wave, w_extra])
+            flux_nm = np.hstack([flux_nm, flux_extra])
+            print('extending wavelengths')"""
 
         if photons:
             h = 6.6260755e-27	 # erg s
             c = 2.99792458e10    # cm/s
-            w_cm = wave/1e7
-            photon_energy = h*c/w_cm
-            flux = flux_nm/photon_energy
+            w_cm = wave / 1e7
+            photon_energy = h * c / w_cm
+            flux = flux_nm / photon_energy
         else:
             flux = flux_nm
 
         if R is not None:
             wave, flux = bintoR(wave, flux, R=R)
         preloaded[key] = wave, flux
+
     return wave, flux
 
 
-def read_phoenix(Teff=5800, logg=4.5, metallicity=0.0, photons=True, R=None):
+def read_phoenix(Teff=5800, logg=4.5, metallicity=0.0, photons=True, R=None, extend_wavelengths=False):
     try:
-        w, f = read_exact_phoenix(Teff=Teff, logg=logg, metallicity=metallicity, photons=photons, R=R)
+        w, f = read_exact_phoenix(
+            Teff=Teff,
+            logg=logg,
+            metallicity=metallicity,
+            photons=photons,
+            R=R,
+            extend_wavelengths=extend_wavelengths
+        )
     except FileNotFoundError:
-        #print('The exact parameters {} were not found in {}'.format(locals(), phoenix_directory))
+        # print('The exact parameters {} were not found in {}'.format(locals(), phoenix_directory))
 
         Teffs, loggs = availability_by_metallicity[metallicity]
         # figure out the closest gravity
         best_gravity = find_nearest(loggs, logg)
-        if best_gravity != logg:
-            print('nudged logg from {} to {}'.format(logg, best_gravity))
+        """if best_gravity != logg:
+            print(
+                "nudged logg from {} to {}".format(
+                    logg, best_gravity
+                )
+            )"""
 
         Teffs = Teffs[loggs == best_gravity]
         close_temperatures = find_two_nearest(Teffs, Teff, verbose=False)
         weights = interpolation_weights(close_temperatures, Teff)
 
-        w_one, f_one = read_exact_phoenix(Teff=close_temperatures[0], logg=best_gravity, metallicity=metallicity, photons=photons, R=R)
-        w_other, f_other = read_exact_phoenix(Teff=close_temperatures[1], logg=best_gravity, metallicity=metallicity, photons=photons, R=R)
-        assert((w_one == w_other).all())
+        w_one, f_one = read_exact_phoenix(
+            Teff=close_temperatures[0],
+            logg=best_gravity,
+            metallicity=metallicity,
+            photons=photons,
+            R=R,
+            extend_wavelengths=extend_wavelengths
+        )
+        w_other, f_other = read_exact_phoenix(
+            Teff=close_temperatures[1],
+            logg=best_gravity,
+            metallicity=metallicity,
+            photons=photons,
+            R=R,
+            extend_wavelengths=extend_wavelengths
+        )
+        assert (w_one == w_other).all()
         w = w_one
         # do logarithmic interpolation
-        f = np.exp(weights[0]*np.log(f_one) + weights[1]*np.log(f_other))
+        f = np.exp(weights[0] * np.log(f_one) + weights[1] * np.log(f_other))
 
     return w, f
```

### Comparing `rainbow-connection-0.0.6/rainbowconnection/sources/phoenix/star.py` & `rainbow-connection-0.0.7/rainbowconnection/sources/sun.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-from ..spectrum import *
-from .library import read_phoenix
+from .thermal import *
 
-class Star(Spectrum):
 
-    def __init__(self, teff=5800*u.K, radius=1*u.Rsun, mass=1*u.Msun, metallicity=0.0, R=None):
-
-        self.teff = teff
-        self.radius = radius
-        self.mass = mass
-        self.logg = np.log10((con.G*self.mass/self.radius**2).to('cm/s**2').value)
-        self.metallicity = metallicity
-
-
-        w, f = read_phoenix(self.teff.to('K').value, logg=self.logg, metallicity=self.metallicity, R=R, photons=False)
-        self._wavelength = w*u.nm
-        self._flux = (f*u.erg/u.s/u.cm**2/u.nm).to(u.W/u.nm/u.m**2)
+class Sun(Spectrum):
+    def __init__(self):
+        self.radius = 1 * u.Rsun
+        self.teff = (
+            (u.Lsun / (con.sigma_sb * 4 * np.pi * u.Rsun ** 2)) ** (1.0 / 4.0)
+        ).to(u.K)
+
+        filename = os.path.join(data_directory, "solarspectrum.txt")
+        d = ascii.read(filename, comment="#")
+        self._wavelength = d["wavelength"].data * u.nm
+        factor = ((1 * u.au) ** 2 / (1 * u.Rsun) ** 2).decompose()
+        self._flux = d["irradiance"].data * u.W / u.nm / u.m ** 2 * factor
         self.default_wavelengths = self._wavelength
 
-        # FIXME -- check if it's surface flux or something else!??!?!
-
-
-    """
     def integrate(self, lower=None, upper=None):
-        '''
+        """
         Integrate the spectrum over wavelength.
 
         It gives a number with units identical to the results of
         `.spectrum()` but without the wavelength (W or W/m**2).
 
         Parameters
         ----------
@@ -36,16 +30,15 @@
         upper : astropy.units.quantity.Quantity
             The lower wavelength limit.
 
         Returns
         -------
         integral : astropy.units.quantity.Quantity
             The integral over wavelength.
-        '''
+        """
 
         # if wavelength limits are used, revert back to the numerical integral
         if (lower is not None) or (upper is not None):
             return super().integrate(lower=lower, upper=upper)
 
         # if there are infinite wavelength limits, use bolometric
-        return 1*u.Lsun/self.normalization()
-    """
+        return 1 * u.Lsun / self.normalization()
```

### Comparing `rainbow-connection-0.0.6/setup.py` & `rainbow-connection-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     # what other packages are needed? (must be pip-installable)
     install_requires=['numpy',
                       'scipy',
                       'ipython',
                       'matplotlib>=3.0',
                       'jupyter',
                       'astropy>=4.0',
-                      'colour-science>=0.3.15',
+                      'colour-science>=0.3.16',
                       'tqdm'],
     # what version of Python is required?
     python_requires='>=3.6',
     # requirements in `key` will install with `pip install rainbow-connection[key]`
     extras_require={},
     # (I think just leave this set to False)
     zip_safe=False,
```

