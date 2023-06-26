# Comparing `tmp/gascompressibility-0.1.1.tar.gz` & `tmp/gascompressibility-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.1.1.tar", last modified: Sat Jun 17 04:36:11 2023, max compression
+gzip compressed data, was "gascompressibility-0.1.2.tar", last modified: Mon Jun 26 15:29:29 2023, max compression
```

## Comparing `gascompressibility-0.1.1.tar` & `gascompressibility-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.097356 gascompressibility-0.1.1/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    11101 2023-06-17 04:36:11.097356 gascompressibility-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10123 2023-06-11 23:32:19.000000 gascompressibility-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.042840 gascompressibility-0.1.1/gascompressibility/
--rw-rw-rw-   0        0        0      220 2023-06-10 23:57:14.000000 gascompressibility-0.1.1/gascompressibility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.065356 gascompressibility-0.1.1/gascompressibility/pseudocritical/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:11:20.000000 gascompressibility-0.1.1/gascompressibility/pseudocritical/__init__.py
--rw-rw-rw-   0        0        0    14942 2023-06-17 04:32:50.000000 gascompressibility-0.1.1/gascompressibility/pseudocritical/piper.py
--rw-rw-rw-   0        0        0    16503 2023-06-17 04:32:50.000000 gascompressibility-0.1.1/gascompressibility/pseudocritical/sutton.py
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.066357 gascompressibility-0.1.1/gascompressibility/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.1/gascompressibility/utilities/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.1/gascompressibility/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.094356 gascompressibility-0.1.1/gascompressibility/z_correlation/
--rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/DAK.py
--rw-rw-rw-   0        0        0        0 2023-06-10 02:22:58.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/hall_yarborough.py
--rw-rw-rw-   0        0        0     1871 2023-06-11 04:54:16.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/kareem.py
--rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/londono.py
--rw-rw-rw-   0        0        0     1463 2023-06-11 05:13:08.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/z_helper.py
--rw-rw-rw-   0        0        0    24973 2023-05-31 14:14:57.000000 gascompressibility-0.1.1/gascompressibility/zfactor.py
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.062358 gascompressibility-0.1.1/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0    11101 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 04:36:11.098356 gascompressibility-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1428 2023-06-17 04:36:08.000000 gascompressibility-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.096356 gascompressibility-0.1.1/tests/
--rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0    32379 2023-06-17 04:35:39.000000 gascompressibility-0.1.1/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.668556 gascompressibility-0.1.2/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    11101 2023-06-26 15:29:29.667557 gascompressibility-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10123 2023-06-11 23:32:19.000000 gascompressibility-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.620373 gascompressibility-0.1.2/gascompressibility/
+-rw-rw-rw-   0        0        0      209 2023-06-26 15:23:51.000000 gascompressibility-0.1.2/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.639373 gascompressibility-0.1.2/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0       56 2023-06-26 15:01:56.000000 gascompressibility-0.1.2/gascompressibility/pseudocritical/__init__.py
+-rw-rw-rw-   0        0        0    16824 2023-06-26 14:37:39.000000 gascompressibility-0.1.2/gascompressibility/pseudocritical/piper.py
+-rw-rw-rw-   0        0        0    14756 2023-06-26 14:32:56.000000 gascompressibility-0.1.2/gascompressibility/pseudocritical/sutton.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.644373 gascompressibility-0.1.2/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.2/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.2/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.661554 gascompressibility-0.1.2/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.2/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.2/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.2/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.2/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.2/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0     6067 2023-06-26 15:23:51.000000 gascompressibility-0.1.2/gascompressibility/z_correlation/z_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.637374 gascompressibility-0.1.2/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    11101 2023-06-26 15:29:29.000000 gascompressibility-0.1.2/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-06-26 15:29:29.000000 gascompressibility-0.1.2/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:29:29.000000 gascompressibility-0.1.2/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-26 15:29:29.000000 gascompressibility-0.1.2/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-26 15:29:29.000000 gascompressibility-0.1.2/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:29:29.668556 gascompressibility-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1472 2023-06-26 15:29:09.000000 gascompressibility-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:29:29.666556 gascompressibility-0.1.2/tests/
+-rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0    30832 2023-06-26 15:02:48.000000 gascompressibility-0.1.2/tests/test_gascomp.py
```

### Comparing `gascompressibility-0.1.1/LICENSE` & `gascompressibility-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.1/PKG-INFO` & `gascompressibility-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.1
+Version: 0.1.2
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.1/README.md` & `gascompressibility-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.1/gascompressibility/pseudocritical/piper.py` & `gascompressibility-0.1.2/gascompressibility/pseudocritical/piper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,152 +1,298 @@
 import numpy as np
-from scipy import optimize
 import matplotlib.pyplot as plt
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
 from gascompressibility.utilities.utilities import calc_psig_to_psia
-from gascompressibility.z_correlation.z_helper import get_z_model
+
+"""
+This is a piper module
+"""
 
 
 class piper(object):
-    def __init__(
-            self,
-            Pc_H2S=1306,
-            Tc_H2S=672.3,
-            Pc_CO2=1071,
-            Tc_CO2=547.5,
-            Pc_N2=492.4,
-            Tc_N2=227.16,
-    ):
+    """
+    An example docstring for a class definition.
+    """
+
+    def __init__(self):
+
         self.mode = 'piper'
         self._check_invalid_mode(self.mode)  # prevent user modification of self.mode
 
         self.sg = None
         self.T_f = None
         self.T = None
         self.P = None
         self.H2S = None
         self.CO2 = None
         self.N2 = None
 
-        self.Pc_H2S = Pc_H2S
-        self.Tc_H2S = Tc_H2S
-        self.Pc_CO2 = Pc_CO2
-        self.Tc_CO2 = Tc_CO2
-        self.Pc_N2 = Pc_N2
-        self.Tc_N2 = Tc_N2
+        self.Pc_H2S = 1306
+        self.Tc_H2S = 672.3
+        self.Pc_CO2 = 1071
+        self.Tc_CO2 = 547.5
+        self.Pc_N2 = 492.4
+        self.Tc_N2 = 227.16
+
         self.Tpc = None
         self.Ppc = None
         self.J = None
         self.K = None
         self.Tr = None
         self.Pr = None
 
-        self.Z = None
+        self.ps_props = {
+            'Tpc': self.Tpc,
+            'Ppc': self.Ppc,
+            'J': self.J,
+            'K': self.K,
+            'Tr': self.Tr,
+            'Pr': self.Pr,
+        }
 
         self._first_caller_name = None
         self._first_caller_keys = {}
         self._first_caller_kwargs = {}
         self._first_caller_is_saved = False
 
-
-
     def __str__(self):
-        return str(self.Z)
+        return str(self.ps_props)
 
     def __repr__(self):
-        return '<GasCompressibilityFactor object. Mixing Rule = %s>' % self.mode
+        return str(self.ps_props)
 
-    """Stewart-Burkhardt-VOO parameter J, (°R/psia)"""
     def calc_J(self, sg=None, H2S=None, CO2=None, N2=None):
+
+        """
+        Calculates the Stewart-Burkhardt-VOO parameter J, (°R/psia)
+
+        Parameters
+        ----------
+        sg : float
+            specific gravity of gas (dimensionless)
+        H2S : float
+            mole fraction of H2S (dimensionless)
+        CO2 : float
+            mole fraction of CO2 (dimensionless)
+        N2 : float
+            mole fraction of N2 (dimensionless)
+
+        Returns
+        -------
+        float
+            SBV parameter, J, (°R/psia)
+        """
+
+
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_sg(sg)
         self._initialize_H2S(H2S)
         self._initialize_CO2(CO2)
         self._initialize_N2(N2)
         self.J = 0.11582 \
                  - 0.45820 * self.H2S * (self.Tc_H2S / self.Pc_H2S) \
                  - 0.90348 * self.CO2 * (self.Tc_CO2 / self.Pc_CO2) \
                  - 0.66026 * self.N2 * (self.Tc_N2 / self.Pc_N2) \
                  + 0.70729 * self.sg \
                  - 0.099397 * self.sg ** 2
+        self.ps_props['J'] = self.J
         return self.J
 
-    """Stewart-Burkhardt-VOO parameter K, (°R/psia^0.5)"""
     def calc_K(self, sg=None, H2S=None, CO2=None, N2=None):
+        """
+        Calculates the Stewart-Burkhardt-VOO parameter K, (°R/psia^0.5)
+
+        Parameters
+        ----------
+        sg : float
+            specific gravity of gas (dimensionless)
+        H2S : float
+            mole fraction of H2S (dimensionless)
+        CO2 : float
+            mole fraction of CO2 (dimensionless)
+        N2 : float
+            mole fraction of N2 (dimensionless)
+
+        Returns
+        -------
+        float
+            SBV parameter, K, (°R/psia^0.5)
+        """
+
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_sg(sg)
         self._initialize_H2S(H2S)
         self._initialize_CO2(CO2)
         self._initialize_N2(N2)
         self.K = 3.8216 \
                  - 0.06534 * self.H2S * (self.Tc_H2S / np.sqrt(self.Pc_H2S)) \
                  - 0.42113 * self.CO2 * (self.Tc_CO2 / np.sqrt(self.Pc_CO2)) \
                  - 0.91249 * self.N2 * (self.Tc_N2 / np.sqrt(self.Pc_N2)) \
                  + 17.438 * self.sg \
                  - 3.2191 * self.sg ** 2
+        self.ps_props['K'] = self.K
         return self.K
 
     """pseudo-critical temperature (°R)"""
     def calc_Tpc(self, sg=None, H2S=None, CO2=None, N2=None, J=None, K=None, ignore_conflict=False):
+        """
+        Calculates pseudo-critical temperature, Tpc (°R)
+
+        Parameters
+        ----------
+        sg : float
+            specific gravity of gas (dimensionless)
+        H2S : float
+            mole fraction of H2S (dimensionless)
+        CO2 : float
+            mole fraction of CO2 (dimensionless)
+        N2 : float
+            mole fraction of N2 (dimensionless)
+        J : float
+            SBV parameter, J, (°R/psia)
+        K : float
+            SBV parameter, K, (°R/psia^0.5)
+        ignore_conflict : bool
+            set this to True to force usage of input variables instead of calculated variables.
+        Returns
+        -------
+        float
+            Pseudo-critical temperature, Tpc (°R)
+        """
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_J(J, sg=sg, H2S=H2S, CO2=CO2, N2=N2, ignore_conflict=ignore_conflict)
         self._initialize_K(K, sg=sg, H2S=H2S, CO2=CO2, N2=N2, ignore_conflict=ignore_conflict)
         self.Tpc = self.K ** 2 / self.J
+        self.ps_props['Tpc'] = self.Tpc
         return self.Tpc
 
-    """pseudo-critical pressure (psi)"""
     def calc_Ppc(self, sg=None, H2S=None, CO2=None, N2=None, J=None, K=None, Tpc=None, ignore_conflict=False):
+        """
+        Calculates pseudo-critical pressure, Ppc (psia)
+
+        Parameters
+        ----------
+        sg : float
+            specific gravity of gas (dimensionless)
+        H2S : float
+            mole fraction of H2S (dimensionless)
+        CO2 : float
+            mole fraction of CO2 (dimensionless)
+        N2 : float
+            mole fraction of N2 (dimensionless)
+        J : float
+            SBV parameter, J, (°R/psia)
+        K : float
+            SBV parameter, K, (°R/psia^0.5)
+        Tpc : float
+            pseudo-critical temperature, Tpc (°R)
+        ignore_conflict : bool
+            set this to True to force usage of input variables instead of calculated variables.
+
+        Returns
+        -------
+        float
+            pseudo-critical pressure, Ppc (psia)
+        """
+
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
 
         if Tpc is not None:
             if K is not None:
                 raise TypeError('%s() has conflicting keyword arguments "%s" and "%s"' % (self._first_caller_name, 'Tpc', 'K'))
             self.Tpc = Tpc  # skips self._check_conflicting_arguments() when initializing Tpc
         else:
             self._initialize_Tpc(Tpc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K, ignore_conflict=ignore_conflict)
 
         self._initialize_J(J, sg=sg, H2S=H2S, CO2=CO2, N2=N2, ignore_conflict=ignore_conflict)
         self.Ppc = self.Tpc / self.J
+        self.ps_props['Ppc'] = self.Ppc
         return self.Ppc
 
-    """pseudo-reduced temperature (°R)"""
     def calc_Tr(self, T=None, sg=None, Tpc=None, H2S=None, CO2=None, N2=None, J=None, K=None, ignore_conflict=False):
+        """
+        Calculates pseudo-reduced temperature, Tr (°R)
+
+        Parameters
+        ----------
+        T : float
+            temperature of gas (°F)
+        sg : float
+            specific gravity of gas (dimensionless)
+        H2S : float
+            mole fraction of H2S (dimensionless)
+        CO2 : float
+            mole fraction of CO2 (dimensionless)
+        N2 : float
+            mole fraction of N2 (dimensionless)
+        J : float
+            SBV parameter, J, (°R/psia)
+        K : float
+            SBV parameter, K, (°R/psia^0.5)
+        ignore_conflict : bool
+            set this to True to force usage of input variables instead of calculated variables.
+
+        Returns
+        -------
+        float
+            pseudo-reduced temperature, Tr (°R)
+
+        """
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_T(T)
         self._initialize_Tpc(Tpc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K, ignore_conflict=ignore_conflict)
         self.Tr = self.T / self.Tpc
+        self.ps_props['Tr'] = self.Tr
         return self.Tr
 
     """pseudo-reduced pressure (psi)"""
-
     def calc_Pr(self, P=None, sg=None, Tpc=None, Ppc=None, H2S=None, CO2=None, N2=None, J=None, K=None, ignore_conflict=False):
+        """
+        Calculates pseudo-reduced pressure, Pr (psia)
+
+        Parameters
+        ----------
+        P : float
+            pressure of gas (psig)
+        sg : float
+            specific gravity of gas (dimensionless)
+        H2S : float
+            mole fraction of H2S (dimensionless)
+        CO2 : float
+            mole fraction of CO2 (dimensionless)
+        N2 : float
+            mole fraction of N2 (dimensionless)
+        J : float
+            SBV parameter, J, (°R/psia)
+        K : float
+            SBV parameter, K, (°R/psia^0.5)
+        ignore_conflict : bool
+            set this to True to force usage of input variables instead of calculated variables.
+
+        Returns
+        -------
+        float
+            pseudo-reduced pressure, Pr (psia)
+        """
+
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_P(P)
         self._initialize_Ppc(Ppc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K, Tpc=Tpc, ignore_conflict=ignore_conflict)
         self.Pr = self.P / self.Ppc
+        self.ps_props['Pr'] = self.Pr
         return self.Pr
 
-    """Newton-Raphson nonlinear solver"""
-    def calc_Z(self, sg=None, P=None, T=None, Tpc=None, Ppc=None, H2S=None, CO2=None, N2=None, Tr=None, Pr=None,
-               J=None, K=None, ignore_conflict=False, model='DAK', guess=0.9, newton_kwargs=None):
-
+    """This function is used by z_helper.py's calc_Z function to check redundant arguments for Pr and Tr"""
+    def _initialize_Tr_and_Pr(self, sg=None, P=None, T=None, Tpc=None, Ppc=None, H2S=None, CO2=None, N2=None, Tr=None, Pr=None, J=None, K=None, ignore_conflict=False):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_Tr(Tr, T=T, sg=sg, Tpc=Tpc, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K, ignore_conflict=ignore_conflict)
         self._initialize_Pr(Pr, P=P, sg=sg, Tpc=Tpc, Ppc=Ppc, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K, ignore_conflict=ignore_conflict)
-
-        z_model = get_z_model(model=model)
-
-        if newton_kwargs is None:
-            self.Z = optimize.newton(z_model, guess, args=(self.Pr, self.Tr))
-        else:
-            self.Z = optimize.newton(z_model, guess, args=(self.Pr, self.Tr), **newton_kwargs)
-
-        return self.Z
+        return self.Tr, self.Pr
 
     def _set_first_caller_attributes(self, func_name, func_kwargs):
         """
         Helper function to set properties related to the first function called (first in the call stack).
         This function doesn't do anything for 'calc_...()' functions called inside the first function.
         For exmaple, if `calc_Pr()' is called, this function is skipped for 'calc_Ppc()' function which is
         triggered inside `calc_Pr()`.
@@ -181,17 +327,21 @@
         :param func: string
             ex1) func_name = "calc_Tpc",
             ex2) func_name = "calc_J",
         :param calculated_var: string
             ex1) calculated_var = 'Tpc'
             ex1) calculated_var = 'J'
         """
-        args = inspect.getfullargspec(func).args[1:]  # arg[0] = 'self'
+        args = inspect.getfullargspec(func).args[1:]  # arg[0] = 'self', args = arguments defined in "func"
         for arg in args:
             if self._first_caller_kwargs[arg] is not None:
+
+                if self._first_caller_name == '_initialize_Tr_and_Pr':
+                    raise TypeError('%s() has conflicting keyword arguments "%s" and "%s"' % ('calc_Z', calculated_var, arg))
+
                 raise TypeError('%s() has conflicting keyword arguments "%s" and "%s"' % (self._first_caller_name, calculated_var, arg))
 
     def _initialize_sg(self, sg):
         if sg is None:
             if self._first_caller_name == 'calc_J' or self._first_caller_name == 'calc_K':
                 raise TypeError("Missing a required argument, sg (specific gravity, dimensionless)")
             else:
@@ -283,66 +433,7 @@
             self.Tr = Tr
 
     def _check_invalid_mode(self, mode):
         if mode != 'sutton' and mode != 'piper':
             raise TypeError("Invalid optional argument, mode (calculation method), input either 'sutton', 'piper'")
         self.mode = mode
 
-    def quickstart(self):
-
-        xmax = 8
-        Prs = np.linspace(0, xmax, xmax * 10 + 1)
-        Prs = np.array([round(Pr, 1) for Pr in Prs])
-
-        Trs = np.array([1.05, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9, 2.0, 2.2, 2.4, 2.6, 2.8, 3.0])
-
-        results = {Tr: {
-            'Pr': np.array([]),
-            'Z': np.array([])
-        } for Tr in Trs}
-
-        for Tr in Trs:
-            for Pr in Prs:
-                z_obj = piper()
-                z = z_obj.calc_Z(Tr=Tr, Pr=Pr, **{'maxiter': 1000})
-                results[Tr]['Z'] = np.append(results[Tr]['Z'], [z], axis=0)
-                results[Tr]['Pr'] = np.append(results[Tr]['Pr'], [Pr], axis=0)
-
-        label_fontsize = 12
-
-        fig, ax = plt.subplots(figsize=(8, 5))
-        for Tr in Trs:
-
-            Zs = results[Tr]['Z']
-            idx_min = np.where(Zs == min(Zs))
-
-            p = ax.plot(Prs, Zs)
-            if Tr == 1.05:
-                t = ax.text(Prs[idx_min] - 0.5, min(Zs) - 0.005, '$T_{r}$ = 1.2', color=p[0].get_color())
-                t.set_bbox(dict(facecolor='white', alpha=0.9, edgecolor='white', pad=1))
-            else:
-                t = ax.text(Prs[idx_min] - 0.2, min(Zs) - 0.005, Tr, color=p[0].get_color())
-                t.set_bbox(dict(facecolor='white', alpha=0.9, edgecolor='white', pad=1))
-
-        ax.set_xlim(0, xmax)
-        ax.minorticks_on()
-        ax.grid(alpha=0.5)
-        ax.grid(b=True, which='minor', alpha=0.1)
-        ax.spines.top.set_visible(False)
-        ax.spines.right.set_visible(False)
-
-        ax.set_ylabel('Compressibility Factor, $Z$', fontsize=label_fontsize)
-        ax.set_xlabel('Pseudo-Reduced Pressure, $P_{r}$', fontsize=label_fontsize)
-        ax.text(0.57, 0.08, '$T_{r}$ = Pseudo-Reduced Temperature', fontsize=11, transform=ax.transAxes,
-                bbox=dict(facecolor='white'))
-
-        def setbold(txt):
-            return ' '.join([r"$\bf{" + item + "}$" for item in txt.split(' ')])
-
-        ax.set_title(setbold('Real Gas Law Compressibility Factor - Z') + ", computed with GasCompressiblityFactor-py ",
-                     fontsize=12, pad=10, x=0.445, y=1.06)
-        ax.annotate('', xy=(-0.09, 1.05), xycoords='axes fraction', xytext=(1.05, 1.05),
-                    arrowprops=dict(arrowstyle="-", color='k'))
-
-        fig.tight_layout()
-
-        return results, fig, ax
```

### Comparing `gascompressibility-0.1.1/gascompressibility/pseudocritical/sutton.py` & `gascompressibility-0.1.2/gascompressibility/pseudocritical/sutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from scipy import optimize
 import matplotlib.pyplot as plt
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
 from gascompressibility.utilities.utilities import calc_psig_to_psia
-from gascompressibility.z_correlation.z_helper import get_z_model
+from gascompressibility.z_correlation import z_helper
 
 
 class sutton:
     def __init__(self):
         self.mode = 'sutton'
         self._check_invalid_mode(self.mode)  # prevent user modification of self.mode
 
@@ -26,26 +26,34 @@
         self.B = None
         self.e_correction = None
         self.Tpc_corrected = None
         self.Ppc_corrected = None
         self.Tr = None
         self.Pr = None
 
-        self.Z = None
+        self.ps_props = {
+            'Tpc': self.Tpc,
+            'Ppc': self.Ppc,
+            'e_correction': self.e_correction,
+            'Tpc_corrected': self.Tpc_corrected,
+            'Ppc_corrected': self.Ppc_corrected,
+            'Tr': self.Tr,
+            'Pr': self.Pr,
+        }
 
         self._first_caller_name = None
         self._first_caller_keys = {}
         self._first_caller_kwargs = {}
         self._first_caller_is_saved = False
 
     def __str__(self):
-        return str(self.Z)
+        return str(self.ps_props)
 
     def __repr__(self):
-        return '<GasCompressibilityFactor object. Mixing Rule = %s>' % self.mode
+        return str(self.ps_props)
 
     """sum of the mole fractions of CO2 and H2S in a gas mixture"""
     def _calc_A(self, H2S=None, CO2=None):
         self._initialize_H2S(H2S)
         self._initialize_CO2(CO2)
         self.A = self.H2S + self.CO2
         return self.A
@@ -57,96 +65,96 @@
         return self.B
 
     """pseudo-critical temperature (°R)"""
     def calc_Tpc(self, sg=None):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_sg(sg)
         self.Tpc = 169.2 + 349.5 * self.sg - 74.0 * self.sg ** 2
+        self.ps_props['Tpc'] = self.Tpc
         return self.Tpc
 
     """pseudo-critical pressure (psi)"""
     def calc_Ppc(self, sg=None):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_sg(sg)
         self.Ppc = 756.8 - 131.07 * self.sg - 3.6 * self.sg ** 2
+        self.ps_props['Ppc'] = self.Ppc
         return self.Ppc
 
     """correction for CO2 and H2S (°R)"""
     def calc_e_correction(self, H2S=None, CO2=None):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_A(A=None, H2S=H2S, CO2=CO2)
         self._initialize_B(B=None, H2S=H2S)
         self.e_correction = 120 * (self.A ** 0.9 - self.A ** 1.6) + 15 * (self.B ** 0.5 - self.B ** 4)
+        self.ps_props['e_correction'] = self.e_correction
         return self.e_correction
 
     def calc_Tpc_corrected(self, sg=None, Tpc=None, e_correction=None, H2S=None, CO2=None, ignore_conflict=False):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_Tpc(Tpc, sg=sg)
 
         # Correction is not needed if no sour gas is present
         if e_correction is None and H2S is None and CO2 is None:
             self.Tpc_corrected = self.Tpc
+            self.ps_props['Tpc_corrected'] = self.Tpc_corrected
             return self.Tpc_corrected
 
         self._initialize_e_correction(e_correction, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
         self.Tpc_corrected = self.Tpc - self.e_correction
+        self.ps_props['Tpc_corrected'] = self.Tpc_corrected
         return self.Tpc_corrected
 
     """ corrected pseudo-critical pressure (psi)"""
     def calc_Ppc_corrected(self, sg=None, Tpc=None, Ppc=None, e_correction=None, Tpc_corrected=None, H2S=None, CO2=None, ignore_conflict=False):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_Ppc(Ppc, sg=sg)
 
         # Correction is not needed if no sour gas is present
         if e_correction is None and H2S is None and CO2 is None and Tpc is None and Tpc_corrected is None:
             self.Ppc_corrected = self.Ppc
+            self.ps_props['Ppc_corrected'] = self.Ppc_corrected
             return self.Ppc_corrected
 
         self._initialize_Tpc(Tpc, sg=sg)
         self._initialize_B(B=None, H2S=H2S)
         self._initialize_e_correction(e_correction, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
         self._initialize_Tpc_corrected(Tpc_corrected, sg=sg, Tpc=Tpc, e_correction=e_correction, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
         self.Ppc_corrected = (self.Ppc * self.Tpc_corrected) / (self.Tpc - self.B * (1 - self.B) * self.e_correction)
+        self.ps_props['Ppc_corrected'] = self.Ppc_corrected
         return self.Ppc_corrected
 
     """pseudo-reduced temperature (°R)"""
     def calc_Tr(self, T=None, Tpc_corrected=None, sg=None, Tpc=None, e_correction=None, H2S=None, CO2=None, ignore_conflict=False):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_T(T)
         self._initialize_Tpc_corrected(Tpc_corrected, sg=sg, Tpc=Tpc, e_correction=e_correction, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
         self.Tr = self.T / self.Tpc_corrected
+        self.ps_props['Tr'] = self.Tr
         return self.Tr
 
     """pseudo-reduced pressure (psi)"""
     def calc_Pr(self, P=None, Ppc_corrected=None, sg=None, Tpc=None, Ppc=None, e_correction=None, Tpc_corrected=None, H2S=None, CO2=None, ignore_conflict=False):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_P(P)
         self._initialize_Ppc_corrected(Ppc_corrected, sg=sg, Tpc=Tpc, Ppc=Ppc, e_correction=e_correction, Tpc_corrected=Tpc_corrected, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
         self.Pr = self.P / self.Ppc_corrected
+        self.ps_props['Pr'] = self.Pr
         return self.Pr
 
-    """Newton-Raphson nonlinear solver"""
-    def calc_Z(self, sg=None, P=None, T=None, Tpc=None, Ppc=None, Tpc_corrected=None, Ppc_corrected=None,
-               H2S=None, CO2=None, Tr=None, Pr=None, e_correction=None, ignore_conflict=False,
-               model='DAK', guess=0.9, newton_kwargs=None):
-
+    """This function is used by z_helper.py's calc_Z function to check redundant arguments for Pr and Tr"""
+    def _initialize_Tr_and_Pr(self, sg=None, P=None, T=None, Tpc=None, Ppc=None, Tpc_corrected=None, Ppc_corrected=None,
+               H2S=None, CO2=None, Tr=None, Pr=None, e_correction=None, ignore_conflict=False):
         self._set_first_caller_attributes(inspect.stack()[0][3], locals())
         self._initialize_Tr(Tr, T, Tpc_corrected=Tpc_corrected, sg=sg, Tpc=Tpc, e_correction=e_correction, H2S=H2S,
                             CO2=CO2, ignore_conflict=ignore_conflict)
         self._initialize_Pr(Pr, P=P, Ppc_corrected=Ppc_corrected, sg=sg, Tpc=Tpc, Ppc=Ppc, e_correction=e_correction,
                             Tpc_corrected=Tpc_corrected, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
+        return self.Tr, self.Pr
 
-        z_model = get_z_model(model=model)
-
-        if newton_kwargs is None:
-            self.Z = optimize.newton(z_model, guess, args=(self.Pr, self.Tr))
-        else:
-            self.Z = optimize.newton(z_model, guess, args=(self.Pr, self.Tr), **newton_kwargs)
-
-        return self.Z
 
     def _set_first_caller_attributes(self, func_name, func_kwargs):
         """
         Helper function to set properties related to the first function called (first in the call stack).
         This function doesn't do anything for 'calc_...()' functions called inside the first function.
         For exmaple, if `calc_Ppc_corrected()' is called, this function is skipped for 'calc_Ppc()' function which is
         triggered inside `calc_Ppc_corrected()`.
@@ -185,14 +193,18 @@
             ex1) calculated_var = 'Tpc'
             ex1) calculated_var = 'J'
         """
 
         args = inspect.getfullargspec(func).args[1:]  # arg[0] = 'self', args = arguments defined in "func"
         for arg in args:
             if self._first_caller_kwargs[arg] is not None:
+
+                if self._first_caller_name == '_initialize_Tr_and_Pr':
+                    raise TypeError('%s() has conflicting keyword arguments "%s" and "%s"' % ('calc_Z', calculated_var, arg))
+
                 raise TypeError('%s() has conflicting keyword arguments "%s" and "%s"' % (self._first_caller_name, calculated_var, arg))
 
     def _initialize_sg(self, sg):
         if sg is None:
             if self._first_caller_name == 'calc_Ppc' or self._first_caller_name == 'calc_Tpc':
                 raise TypeError("Missing a required argument, sg (specific gravity, dimensionless)")
             else:
@@ -297,68 +309,9 @@
             self.Tr = Tr
 
     def _check_invalid_mode(self, mode):
         if mode != 'sutton' and mode != 'piper':
             raise TypeError("Invalid optional argument, mode (calculation method), input either 'sutton', 'piper', or None (default='sutton')")
         self.mode = mode
 
-    def quickstart(self):
-
-        xmax = 8
-        Prs = np.linspace(0, xmax, xmax * 10 + 1)
-        Prs = np.array([round(Pr, 1) for Pr in Prs])
-
-        Trs = np.array([1.05, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9, 2.0, 2.2, 2.4, 2.6, 2.8, 3.0])
-
-        results = {Tr: {
-            'Pr': np.array([]),
-            'Z': np.array([])
-        } for Tr in Trs}
-
-        for Tr in Trs:
-            for Pr in Prs:
-                z_obj = sutton()
-                z = z_obj.calc_Z(Tr=Tr, Pr=Pr, **{'maxiter': 1000})
-                results[Tr]['Z'] = np.append(results[Tr]['Z'], [z], axis=0)
-                results[Tr]['Pr'] = np.append(results[Tr]['Pr'], [Pr], axis=0)
-
-        label_fontsize = 12
-
-        fig, ax = plt.subplots(figsize=(8, 5))
-        for Tr in Trs:
-
-            Zs = results[Tr]['Z']
-            idx_min = np.where(Zs == min(Zs))
-
-            p = ax.plot(Prs, Zs)
-            if Tr == 1.05:
-                t = ax.text(Prs[idx_min] - 0.5, min(Zs) - 0.005, '$T_{r}$ = 1.2', color=p[0].get_color())
-                t.set_bbox(dict(facecolor='white', alpha=0.9, edgecolor='white', pad=1))
-            else:
-                t = ax.text(Prs[idx_min] - 0.2, min(Zs) - 0.005, Tr, color=p[0].get_color())
-                t.set_bbox(dict(facecolor='white', alpha=0.9, edgecolor='white', pad=1))
-
-        ax.set_xlim(0, xmax)
-        ax.minorticks_on()
-        ax.grid(alpha=0.5)
-        ax.grid(b=True, which='minor', alpha=0.1)
-        ax.spines.top.set_visible(False)
-        ax.spines.right.set_visible(False)
-
-        ax.set_ylabel('Compressibility Factor, $Z$', fontsize=label_fontsize)
-        ax.set_xlabel('Pseudo-Reduced Pressure, $P_{r}$', fontsize=label_fontsize)
-        ax.text(0.57, 0.08, '$T_{r}$ = Pseudo-Reduced Temperature', fontsize=11, transform=ax.transAxes,
-                bbox=dict(facecolor='white'))
-
-        def setbold(txt):
-            return ' '.join([r"$\bf{" + item + "}$" for item in txt.split(' ')])
-
-        ax.set_title(setbold('Real Gas Law Compressibility Factor - Z') + ", computed with GasCompressiblityFactor-py ",
-                     fontsize=12, pad=10, x=0.445, y=1.06)
-        ax.annotate('', xy=(-0.09, 1.05), xycoords='axes fraction', xytext=(1.05, 1.05),
-                    arrowprops=dict(arrowstyle="-", color='k'))
-
-        fig.tight_layout()
-
-        return results, fig, ax
```

### Comparing `gascompressibility-0.1.1/gascompressibility/z_correlation/DAK.py` & `gascompressibility-0.1.2/gascompressibility/z_correlation/DAK.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.1/gascompressibility/z_correlation/hall_yarborough.py` & `gascompressibility-0.1.2/gascompressibility/z_correlation/hall_yarborough.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.1/gascompressibility/z_correlation/londono.py` & `gascompressibility-0.1.2/gascompressibility/z_correlation/londono.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.1/gascompressibility.egg-info/PKG-INFO` & `gascompressibility-0.1.2/gascompressibility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.1
+Version: 0.1.2
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.1/gascompressibility.egg-info/SOURCES.txt` & `gascompressibility-0.1.2/gascompressibility.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 gascompressibility/__init__.py
-gascompressibility/zfactor.py
 gascompressibility.egg-info/PKG-INFO
 gascompressibility.egg-info/SOURCES.txt
 gascompressibility.egg-info/dependency_links.txt
 gascompressibility.egg-info/requires.txt
 gascompressibility.egg-info/top_level.txt
 gascompressibility/pseudocritical/__init__.py
 gascompressibility/pseudocritical/piper.py
```

### Comparing `gascompressibility-0.1.1/setup.py` & `gascompressibility-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
         "notes.py",
         "custom.svg",
         "testruns.ipynb",
         "papers",
+        "docs",
+        "docs_save_6_24",
     ]),
     description='GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     classifiers=classifiers(),
     license='MIT',
     author='Eric Kim',
```

