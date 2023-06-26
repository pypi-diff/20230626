# Comparing `tmp/pymcabc-0.3.0.tar.gz` & `tmp/pymcabc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcabc-0.3.0.tar", last modified: Sun Jun 25 14:26:51 2023, max compression
+gzip compressed data, was "pymcabc-0.5.0.tar", last modified: Mon Jun 26 10:44:00 2023, max compression
```

## Comparing `pymcabc-0.3.0.tar` & `pymcabc-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.880414 pymcabc-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-25 14:26:43.000000 pymcabc-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-25 14:26:43.000000 pymcabc-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-25 14:26:51.876414 pymcabc-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-25 14:26:43.000000 pymcabc-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.876414 pymcabc-0.3.0/pymcabc/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/cross_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/decay_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/feynman_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/generate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/identify_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/save_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.876414 pymcabc-0.3.0/pymcabc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 14:26:51.880414 pymcabc-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-25 14:26:43.000000 pymcabc-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.876414 pymcabc-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_crosssection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_evengen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_identify.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 10:43:51.000000 pymcabc-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 10:43:51.000000 pymcabc-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 10:44:00.261516 pymcabc-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-26 10:43:51.000000 pymcabc-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/pymcabc/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/decay_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/feynman_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/generate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/identify_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-06-26 10:43:51.000000 pymcabc-0.5.0/pymcabc/save_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/pymcabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 10:44:00.000000 pymcabc-0.5.0/pymcabc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:44:00.261516 pymcabc-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-26 10:43:51.000000 pymcabc-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:44:00.261516 pymcabc-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_evengen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 10:43:51.000000 pymcabc-0.5.0/tests/test_plot.py
```

### Comparing `pymcabc-0.3.0/LICENSE` & `pymcabc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcabc-0.3.0/PKG-INFO` & `pymcabc-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.3.0
+Version: 0.5.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,15 @@
 1. Import pymcabc:
 ```python
 import pymcabc
 ```
 
 1. Define the process, for example:
 ```python
-pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,Ecm=30)
+pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,pi=30)
 ```
 
 2. Calculate the total cross section of the process (in barn):
 ```python
 pymcabc.CrossSection().calc_xsection()
 ```
```

### Comparing `pymcabc-0.3.0/README.md` & `pymcabc-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 1. Import pymcabc:
 ```python
 import pymcabc
 ```
 
 1. Define the process, for example:
 ```python
-pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,Ecm=30)
+pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,pi=30)
 ```
 
 2. Calculate the total cross section of the process (in barn):
 ```python
 pymcabc.CrossSection().calc_xsection()
 ```
```

### Comparing `pymcabc-0.3.0/pymcabc/cross_section.py` & `pymcabc-0.5.0/pymcabc/cross_section.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,41 +15,56 @@
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.mx = library["mx"][0]
         self.Ecm = library["Ecm"][0]
         self.g = pymcabc.constants.g
         self.pi = pymcabc.constants.pi
         self.delta = pymcabc.constants.delta
-        self.p_i = math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
+        self.p_i = library["pi"][0]  # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
 
     def s_channel(self):
         """definition for s channel"""
-        return (self.g**2) / (self.Ecm**2 - self.mx**2)
+        # deno = self.Ecm**2 - self.mx**2
+        deno = (self.p_i**2 + self.m1**2) * (self.p_i**2 + self.m2**2)
+        deno = math.sqrt(deno)
+        deno = deno + self.m1**2 + self.m2**2
+        if abs(deno) <= 0.09:
+            return (self.g**2) / (deno + 100)
+        else:
+            return (self.g**2) / deno
 
     def t_channel(self, costh, pf):
         """definition for t channel"""
         deno = (
             self.m1**2
             + self.m3**2
             - self.mx**2
-            - (self.Ecm * math.sqrt(pf**2 + self.m3**2))
+            - (
+                2
+                * math.sqrt(self.p_i**2 + self.m1**2)
+                * math.sqrt(pf**2 + self.m3**2)
+            )
             + (2 * self.p_i * pf * costh)
         )
         if abs(deno) <= 0.09:
             return (self.g**2) / (deno + 100)
         else:
             return (self.g**2) / deno
 
     def u_channel(self, costh, pf):
         """definition for u channel"""
         deno = (
             self.m1**2
             + self.m4**2
             - self.mx**2
-            - (self.Ecm * math.sqrt(pf**2 + self.m4**2))
+            - (
+                2
+                * math.sqrt(self.p_i**2 + self.m1**2)
+                * math.sqrt(pf**2 + self.m4**2)
+            )
             - (2 * self.p_i * pf * costh)
         )
         if abs(deno) <= 0.09:
             return (self.g**2) / (deno + 100)
         else:
             return (self.g**2) / deno
 
@@ -66,15 +81,15 @@
             library = json.load(f)
         self.Ecm = library["Ecm"][0]
         self.m1 = library["m1"][0]
         self.m3 = library["m3"][0]
         self.m4 = library["m4"][0]
         self.process = library["process_type"][0]
         self.p_f = pymcabc.constants.outgoing_p(self.Ecm, self.m3, self.m4)
-        self.p_i = math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
+        self.p_i = library["pi"][0]  # math.sqrt((self.Ecm / 2) ** 2 - (self.m1) ** 2)
         self.channel = library["channel"][0]
 
     def dsigma_st(self, costh):
         if self.channel == "s":
             ME = MatrixElement().s_channel()
         elif self.channel == "t":
             ME = MatrixElement().t_channel(costh, self.p_f)
@@ -129,13 +144,13 @@
     def calc_xsection(self, N: int = 40000):
         self.integrate_xsec(N)
         with open("library.json", "r") as f:
             library = json.load(f)
         w_sum = library["w_sum"][0]
         w_square = library["w_square"][0]
         w_max = library["w_max"][0]
-        sigma_x = w_sum * pymcabc.constants.convert / (N * 1e12)
-        variance = math.sqrt(w_square / N - (w_sum / N) ** 2)  # barn unit
+        sigma_x = w_sum * pymcabc.constants.convert / (N * 1e12)  # result in barn unit
+        variance = math.sqrt(abs((w_square / N) - (w_sum / N) ** 2))  # barn unit
         error = (
             variance * pymcabc.constants.convert / (math.sqrt(N) * 1e12)
         )  # barn unit
         return sigma_x, error
```

### Comparing `pymcabc-0.3.0/pymcabc/decay_particle.py` & `pymcabc-0.5.0/pymcabc/decay_particle.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,35 +20,40 @@
         self.decay1_mass = library["decay1_mass"][0]
         self.decay2_mass = library["decay2_mass"][0]
         self.massive = library["massive_mass"][0]
         self.delta = pymcabc.constants.delta
 
     def rotate(self, pdecay: Particle):
         """rotate particle"""
-        costh = (2*random.random()) - 1
+        costh = (2 * random.random()) - 1
         sinth = math.sqrt(1 - costh**2)
         phi = 2 * math.pi * random.random()
         sinPhi = math.sin(phi)
         cosPhi = math.cos(phi)
-        pdecay_out = Particle(0,0,0,0)
-        pdecay_out.px = pdecay.pz * sinth *cosPhi
-        pdecay_out.py = pdecay.pz * sinth *sinPhi
+        pdecay_out = Particle(0, 0, 0, 0)
+        pdecay_out.px = pdecay.pz * sinth * cosPhi
+        pdecay_out.py = pdecay.pz * sinth * sinPhi
         pdecay_out.pz = pdecay.pz * costh
-        pdecay_out.E = pdecay.E 
-        
+        pdecay_out.E = pdecay.E
+
         return pdecay_out
 
     def decay(self, top: Particle):
         """decay particle"""
 
-        E1 = (top.mass()**2 - self.decay2_mass**2 + self.decay1_mass**2)/(2*top.mass())
-        
-        E2 =  top.mass() - E1
+        E1 = (top.mass() ** 2 - self.decay2_mass**2 + self.decay1_mass**2) / (
+            2 * top.mass()
+        )
+
+        E2 = top.mass() - E1
 
-        self.decay_p = math.sqrt((top.mass()**2  - (self.decay1_mass + self.decay2_mass)**2) * (top.mass()**2  - (self.decay1_mass - self.decay2_mass)**2)) / (2*top.mass())
+        self.decay_p = math.sqrt(
+            (top.mass() ** 2 - (self.decay1_mass + self.decay2_mass) ** 2)
+            * (top.mass() ** 2 - (self.decay1_mass - self.decay2_mass) ** 2)
+        ) / (2 * top.mass())
 
         """ 
         self.decay_p = (
             1
             / (2 * top.mass())
             * math.sqrt(
                 (self.mA**4 + self.mB**4 + self.mC**4)
@@ -67,57 +72,56 @@
             self.decay1_mass * self.decay1_mass + self.decay_p * self.decay_p
         ) 
         E2 = math.sqrt(
             self.decay2_mass * self.decay2_mass + self.decay_p * self.decay_p
         ) 
         """
 
-        decay1 = Particle(0,0,0,0)
-        decay2 = Particle(0,0,0,0)
+        decay1 = Particle(0, 0, 0, 0)
+        decay2 = Particle(0, 0, 0, 0)
 
         decay1.set4momenta(E1, 0, 0, self.decay_p)
         decay2.set4momenta(E2, 0, 0, -self.decay_p)
 
         decay1 = self.rotate(decay1)
         decay2.set4momenta(E2, -decay1.px, -decay1.py, -decay1.pz)
-        #decay2 = self.rotate(decay2)
+        # decay2 = self.rotate(decay2)
 
         return decay1, decay2
 
     def nearlyequal(self, a, b):
         if abs(a - b) < 1e-3:
             return True
         else:
             return False
 
     def prepare_decay(self, top: Particle):
         if self.decay_process != "NaN":
             # decay_process = decay_process.replace(" < "," ")
             # decay_process = decay_process.split(" ")
             # print(top.mass()[0], self.massive)
-            decay_array1_px = [0]*len(top.px)
-            decay_array1_py = [0]*len(top.px)
-            decay_array1_pz = [0]*len(top.px)
-            decay_array1_E = [0]*len(top.px)
-
-            decay_array2_px = [0]*len(top.px)
-            decay_array2_py = [0]*len(top.px)
-            decay_array2_pz = [0]*len(top.px)
-            decay_array2_E = [0]*len(top.px)
+            decay_array1_px = [0] * len(top.px)
+            decay_array1_py = [0] * len(top.px)
+            decay_array1_pz = [0] * len(top.px)
+            decay_array1_E = [0] * len(top.px)
+
+            decay_array2_px = [0] * len(top.px)
+            decay_array2_py = [0] * len(top.px)
+            decay_array2_pz = [0] * len(top.px)
+            decay_array2_E = [0] * len(top.px)
 
             for i in range(len(top.px)):
-                heavy_state = Particle(top.E[i],top.px[i], top.py[i],top.pz[i])
-                if self.nearlyequal(heavy_state.mass(), self.massive) and heavy_state.mass() > (
-                    self.decay1_mass + self.decay2_mass
-                ):
-
+                heavy_state = Particle(top.E[i], top.px[i], top.py[i], top.pz[i])
+                if self.nearlyequal(
+                    heavy_state.mass(), self.massive
+                ) and heavy_state.mass() > (self.decay1_mass + self.decay2_mass):
                     decay1, decay2 = self.decay(heavy_state)
                     decay1 = decay1.boost(heavy_state)
                     decay2 = decay2.boost(heavy_state)
-                    
+
                     decay_array1_px[i] = decay1.px
                     decay_array1_py[i] = decay1.py
                     decay_array1_pz[i] = decay1.pz
                     decay_array1_E[i] = decay1.E
 
                     decay_array2_px[i] = decay2.px
                     decay_array2_py[i] = decay2.py
@@ -130,14 +134,15 @@
                     decay_array1_pz[i] = output
                     decay_array1_E[i] = output
 
                     decay_array2_px[i] = output
                     decay_array2_py[i] = output
                     decay_array2_pz[i] = output
                     decay_array2_E[i] = output
-            
-            decay1 = Particle(decay_array1_E,decay_array1_px, decay_array1_py, decay_array1_pz)
-            decay2 = Particle(decay_array2_E,decay_array2_px, decay_array2_py, decay_array2_pz)
-            return decay1, decay2
-
-
 
+            decay1 = Particle(
+                decay_array1_E, decay_array1_px, decay_array1_py, decay_array1_pz
+            )
+            decay2 = Particle(
+                decay_array2_E, decay_array2_px, decay_array2_py, decay_array2_pz
+            )
+            return decay1, decay2
```

### Comparing `pymcabc-0.3.0/pymcabc/detector.py` & `pymcabc-0.5.0/pymcabc/detector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 import random
 import math
 from pymcabc.particle import Particle
 
 
 class Detector:
     """Applies gaussian smearing on E and momenta"""
-    def __init__(self, sigma: float =1., factor: float =1.):
+
+    def __init__(self, sigma: float = 1.0, factor: float = 1.0):
         self.sigma = sigma
         self.factor = factor
 
     def identify_smear(self, particle: Particle, type: str = "gauss"):
         if type == "gauss":
             particle = self.gauss_smear(particle)
         else:
             print("Type Not found")
         return particle
 
     def gauss_smear(self, particle: Particle):
         if particle.px[0] == -9 and particle.py[0] == -9:
             return particle
         else:
-            output_px = [0]*len(particle.px)
-            output_py = [0]*len(particle.px)
-            output_pz = [0]*len(particle.px)
-            output_E = [0]*len(particle.px)
+            output_px = [0] * len(particle.px)
+            output_py = [0] * len(particle.px)
+            output_pz = [0] * len(particle.px)
+            output_E = [0] * len(particle.px)
             for i in range(len(particle.px)):
-                
-                momentum =  math.sqrt(particle.px[i]**2  + particle.py[i]**2  + particle.pz[i]**2 )
-                random_measure_momentum = random.gauss(momentum, self.factor*self.sigma) / momentum
-                random_measure_energy = random.gauss(particle.E[i], self.sigma) / particle.E[i]
-                
-                output_px[i] = random_measure_momentum*particle.px[i]
-                output_py[i] = random_measure_momentum*particle.py[i]
-                output_pz[i] = random_measure_momentum*particle.pz[i]
+                momentum = math.sqrt(
+                    particle.px[i] ** 2 + particle.py[i] ** 2 + particle.pz[i] ** 2
+                )
+                random_measure_momentum = (
+                    random.gauss(momentum, self.factor * self.sigma) / momentum
+                )
+                random_measure_energy = (
+                    random.gauss(particle.E[i], self.sigma) / particle.E[i]
+                )
+
+                output_px[i] = random_measure_momentum * particle.px[i]
+                output_py[i] = random_measure_momentum * particle.py[i]
+                output_pz[i] = random_measure_momentum * particle.pz[i]
 
-                output_E[i] = random_measure_energy*particle.E[i]
+                output_E[i] = random_measure_energy * particle.E[i]
 
                 """output_px[i] = random.gauss(particle.px[i], self.sigma)
                 output_py[i] = random.gauss(particle.py[i], self.sigma)
                 output_pz[i] = random.gauss(particle.pz[i], self.sigma)
                 output_E[i] = random.gauss(particle.E[i], self.sigma)
+
+                mass = output_E[i] ** 2 - (
+                    output_px[i] ** 2 + output_py[i] ** 2 + output_pz[i] ** 2
+                )
                 """
-                mass =  (output_E[i]**2  - (output_px[i]**2 + output_py[i]**2 +output_pz[i]**2 ))
-                print(mass)
+                
             particle_output = Particle(output_E, output_px, output_py, output_pz)
         return particle_output
```

### Comparing `pymcabc-0.3.0/pymcabc/feynman_diagram.py` & `pymcabc-0.5.0/pymcabc/feynman_diagram.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,34 +12,42 @@
     def __init__(self):
         with open("library.json", "r") as f:
             library = json.load(f)
 
         process = library["process"]
         mediator = library["mediator"][0]
         channel = library["channel"][0]
+
+        decay_process = library["decay_process"]
+        if decay_process !="NaN":
+            decay_process = decay_process[0].replace(">","")
+            self.decay_process = decay_process.split()
+            self.decay()
+
         process = process[0].replace(">", mediator)
         self.process = process.split()
+
         if channel == "none":
             for p in library["process_type"][0]:
                 if p == "s":
                     self.s_chan()
                 elif p == "t":
                     self.t_chan()
                 elif p == "u":
                     self.u_chan()
                 else:
                     print("Possible channels: s, t, and u")
                     return 0
         else:
             if channel == "s":
-                    self.s_chan()
+                self.s_chan()
             if channel == "t":
-                    self.t_chan()
+                self.t_chan()
             if channel == "u":
-                    self.u_chan()
+                self.u_chan()
             else:
                 print("Possible channels: s, t, and u")
                 return
 
     def s_chan(self):
         fig = plt.figure(figsize=(5.0, 5.0))
         ax = fig.add_axes([0, 0, 1, 1], frameon=False)
@@ -116,7 +124,27 @@
         b.text(self.process[1], fontsize=20, t=0.1, y=-0.1)
         c.text(self.process[2], fontsize=20)  # ,y=.1)
         d.text(self.process[3], fontsize=20, t=-0.1, y=-0.1)
         e.text(self.process[4], fontsize=20, t=-0.1, y=0.1)
 
         diagram.plot()
         plt.savefig("uchan.pdf")
+
+    def decay(self):
+        fig = plt.figure(figsize=(10.,10.))
+        ax = fig.add_axes([0,0,1,1], frameon=False)
+
+        diagram = Diagram(ax)
+        in1 = diagram.vertex(xy=(.1,.5), marker='')
+        v1  = diagram.vertex(xy=(.5,.5))
+        out1 = diagram.vertex(xy=(.9,.75),marker='')
+        out2 = diagram.vertex(xy=(.9,.25),marker='')
+
+        a = diagram.line(in1,v1,arrow=False)
+        b = diagram.line(v1,out1,arrow=False)
+        c = diagram.line(v1,out2,arrow=False)
+        a.text(self.decay_process[0],fontsize=30,t=.1,y=.1)
+        b.text(self.decay_process[1],fontsize=30,t=-.01,y=.1)
+        c.text(self.decay_process[2],fontsize=30,t=-.1, y=-.1)
+
+        diagram.plot()
+        plt.savefig('decay.pdf')
```

### Comparing `pymcabc-0.3.0/pymcabc/generate_event.py` & `pymcabc-0.5.0/pymcabc/generate_event.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.3.0/pymcabc/identify_process.py` & `pymcabc-0.5.0/pymcabc/identify_process.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import math
 
 
 def build_json():
     library = {
         "mA": [],
         "mB": [],
         "mC": [],
@@ -13,14 +14,15 @@
         "mx": [],
         "massive": [],
         "massive_mass": [],
         "decay_process": [],
         "decay1_mass": [],
         "decay2_mass": [],
         "mediator": [],
+        "pi": [],
         "Ecm": [],
         "process": [],
         "process_type": [],
         "channel": [],
         "w_max": [],
         "w_sum": [],
         "w_square": [],
@@ -37,53 +39,55 @@
     Parameters:
         input_string (str): Physics process. Example > 'A A > B B'
         mA (float): mass of particle A
         mB (float): mass of particle B
         mC (float): mass of particle C
         Ecm (float): center of mass energy
         channel (str): optional, use to study effect a particular channel
-
-
     """
 
     def __init__(
         self,
         input_string: str,
         mA: float,
         mB: float,
         mC: float,
-        Ecm: float,
+        pi: float,
         channel: str = "none",
     ):
         """
         Defines the process, masses of particles and center of mass energy
         Parameters:
             input_string (str): Physics process. Example > 'A A > B B'
             mA (float): mass of particle A
             mB (float): mass of particle B
             mC (float): mass of particle C
             Ecm (float): center of mass energy
             channel (str): optional, use to study effect a particular channel
-
-
         """
 
         build_json()
         with open("library.json", "r") as f:
             self.library = json.load(f)
         self.input_string = input_string
         self.mA = mA
         self.mB = mB
         self.mC = mC
-        self.Ecm = Ecm
+        self.p_i = pi
+        if self.mA < 0 or self.mB < 0 or self.mC < 0:
+            raise Exception("Negative masses not accepted")
+        if self.p_i <= 0:
+            raise Exception("Negative or Zero absolute momentum not accepted")
         self.library["mA"].append(mA)
         self.library["mB"].append(mB)
         self.library["mC"].append(mC)
+        self.library["pi"].append(self.p_i)
         self.library["channel"].append(channel)
         self.process()
+        self.channel()
         self.masses()
         self.ECM()
         self.identify_mediator()
         self.identify_decay()
 
     def process(self):
         """identify the physics process"""
@@ -101,14 +105,27 @@
         else:  # modify logic here; identify valid string at the start
             raise Exception("unable to identify process, please try again")
         self.library["process_type"].append(process_type)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
         return None
 
+    def channel(self):
+        process_type = self.library["process_type"][0]
+        channel = self.library["channel"][0]
+        if channel != "none":
+            if channel not in process_type:
+                raise Exception(
+                    "Channel "
+                    + channel
+                    + " not available for process type "
+                    + process_type
+                )
+        return None
+
     def masses(self):
         """assign masses to m1, m2, m3, m4 and mediator"""
         string = self.input_string.replace(" > ", " ")
         string = string.split(" ")
         pmass = [0, 0, 0, 0]
         for i in range(4):
             if string[i] == "A":
@@ -125,18 +142,25 @@
         self.library["m4"].append(pmass[3])
         with open("library.json", "w") as f:
             json.dump(self.library, f)
         return None
 
     def ECM(self):
         """center of mass energy"""
-        self.library["Ecm"].append(self.Ecm)
+        with open("library.json", "r") as f:
+            library = json.load(f)
+        m1 = library["m1"][0]
+        m2 = library["m2"][0]
+        E1 = math.sqrt(m1**2 + self.p_i**2)
+        E2 = math.sqrt(m2**2 + self.p_i**2)
+        Ecm = E1 + E2
+        self.library["Ecm"].append(Ecm)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
-        return None
+        return Ecm
 
     def identify_mediator(self):
         """identify the mediator of the process"""
         process = self.library["process"][0]
         process = process.replace(" > ", " ")
         if (
             process == "A A B B"
@@ -198,9 +222,8 @@
             self.library["massive"].append("NaN")
             self.library["massive_mass"].append("NaN")
             self.library["decay1_mass"].append("NaN")
             self.library["decay2_mass"].append("NaN")
             self.library["decay_process"].append("NaN")
         with open("library.json", "w") as f:
             json.dump(self.library, f)
-
         return None
```

### Comparing `pymcabc-0.3.0/pymcabc/particle.py` & `pymcabc-0.5.0/pymcabc/particle.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,17 +63,19 @@
         try:
             x = self.E**2 - self.px**2 - self.py**2 - self.pz**2
             if x < 0:
                 x = 0
             else:
                 x = math.sqrt(x)
         except:
-            x = [0]*len(self.px)
+            x = [0] * len(self.px)
             for i in range(len(x)):
-                x[i] = self.E[i]**2 - self.px[i]**2 - self.py[i]**2 - self.pz[i]**2
+                x[i] = (
+                    self.E[i] ** 2 - self.px[i] ** 2 - self.py[i] ** 2 - self.pz[i] ** 2
+                )
                 print(x[i])
                 if x[i] < 0:
                     x[i] = 0
                 else:
                     x[i] = math.sqrt(x)
         return x
 
@@ -87,30 +89,29 @@
     def boost(self, other):
         """
         boosts a particle four momentum.
          # boost motivated from ROOT TLorentzVector class
 
          other is used to boost
         """
-        new = Particle(0., 0., 0., 0.)
-        new_other = Particle(0., 0., 0., 0.)
-        
+        new = Particle(0.0, 0.0, 0.0, 0.0)
+        new_other = Particle(0.0, 0.0, 0.0, 0.0)
+
         new_other.set4momenta(
             other.E, other.px / other.E, other.py / other.E, other.pz / other.E
         )
         beta = new_other.p2()
         gamma = 1.0 / math.sqrt(1.0 - beta)
 
-        if beta>0:
+        if beta > 0:
             gamma_2 = (gamma - 1.0) / beta
         else:
             gamma_2 = 0.0
 
-
         dotproduct = (
             self.px * new_other.px + self.py * new_other.py + self.pz * new_other.pz
         )
         new.px = self.px + (gamma_2 * dotproduct + gamma * self.E) * new_other.px
         new.py = self.py + (gamma_2 * dotproduct + gamma * self.E) * new_other.py
         new.pz = self.pz + (gamma_2 * dotproduct + gamma * self.E) * new_other.pz
         new.E = gamma * (self.E + dotproduct)
-        return new
+        return new
```

### Comparing `pymcabc-0.3.0/pymcabc/save_events.py` & `pymcabc-0.5.0/pymcabc/save_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
     def __init__(
         self,
         Nevent: int,
         boolDecay: bool = True,
         boolDetector: bool = True,
         boolTruth: bool = True,
-        detector_sigma = 1.,
-        detector_factor=1.,
+        detector_sigma=1.0,
+        detector_factor=1.0,
     ):
         """
          saving events
         Parameters:
             Nevent (int): number of events to generate
             boolDecay (bool): optional.  decay particles or not
             boolDetector (bool): optional.  gaussian smearing on particles
             boolTruth (bool): optional.  save truth events
         """
         self.Nevent = Nevent
-        self.detector_sigma  = detector_sigma
-        self.detector_factor  = detector_factor
+        self.detector_sigma = detector_sigma
+        self.detector_factor = detector_factor
 
         with open("library.json", "r") as f:
             library = json.load(f)
         self.w_max = library["w_max"][0]
         self.Ecm = library["Ecm"][0]
         input_string = library["process"][0]
         input_string = input_string.replace(" > ", " ")
@@ -88,16 +88,20 @@
                 self.output_2 + "_Px": self.top2.px,
                 self.output_2 + "_Py": self.top2.py,
                 self.output_2 + "_Pz": self.top2.pz,
             }
 
         if self.boolDecay == False or self.decay_process == "NaN":
             if self.boolDetector == True:
-                self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
-                self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
+                self.top1 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(self.top1)
+                self.top2 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(self.top2)
 
             file = uproot.recreate(name)
             file["events"] = {
                 self.output_1 + "_E": self.top1.E,
                 self.output_1 + "_Px": self.top1.px,
                 self.output_1 + "_Py": self.top1.py,
                 self.output_1 + "_Pz": self.top1.pz,
@@ -109,26 +113,37 @@
         else:
             file = uproot.recreate(name)
             top1 = self.top1
             top2 = self.top2
             decay1, decay2 = DecayParticle().prepare_decay(top1)
             decay3, decay4 = DecayParticle().prepare_decay(top2)
             if self.boolDetector == True:
-
                 if decay1.px[0] == -9 and decay1.E[0] == -9:
-                    self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
+                    self.top1 = Detector(
+                        self.detector_sigma, self.detector_factor
+                    ).gauss_smear(self.top1)
                 if decay2.px[0] == -9 and decay2.E[0] == -9:
-                    self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
-                #self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
-                #self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
-
-                decay1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay1)
-                decay2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay2)
-                decay3 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay3)
-                decay4 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay4)
+                    self.top2 = Detector(
+                        self.detector_sigma, self.detector_factor
+                    ).gauss_smear(self.top2)
+                # self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
+                # self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
+
+                decay1 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(decay1)
+                decay2 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(decay2)
+                decay3 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(decay3)
+                decay4 = Detector(
+                    self.detector_sigma, self.detector_factor
+                ).gauss_smear(decay4)
 
             file["events"] = {
                 self.output_1 + "_E": self.top1.E,
                 self.output_1 + "_Px": self.top1.px,
                 self.output_1 + "_Py": self.top1.py,
                 self.output_1 + "_Pz": self.top1.pz,
                 self.output_1 + "_E_decay_" + self.decayed1: decay1.E,
@@ -147,8 +162,8 @@
                 self.output_2 + "_Px_decay_" + self.decayed1: decay3.px,
                 self.output_2 + "_Py_decay_" + self.decayed1: decay3.py,
                 self.output_2 + "_Pz_decay_" + self.decayed1: decay3.pz,
                 self.output_2 + "_E_decay_" + self.decayed2: decay4.E,
                 self.output_2 + "_Px_decay_" + self.decayed2: decay4.px,
                 self.output_2 + "_Py_decay_" + self.decayed2: decay4.py,
                 self.output_2 + "_Pz_decay_" + self.decayed2: decay4.pz,
-            }
+            }
```

### Comparing `pymcabc-0.3.0/pymcabc.egg-info/PKG-INFO` & `pymcabc-0.5.0/pymcabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.3.0
+Version: 0.5.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,15 @@
 1. Import pymcabc:
 ```python
 import pymcabc
 ```
 
 1. Define the process, for example:
 ```python
-pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,Ecm=30)
+pymcabc.DefineProcess('A A > B B',mA=4,mB=10,mC=1,pi=30)
 ```
 
 2. Calculate the total cross section of the process (in barn):
 ```python
 pymcabc.CrossSection().calc_xsection()
 ```
```

### Comparing `pymcabc-0.3.0/pymcabc.egg-info/SOURCES.txt` & `pymcabc-0.5.0/pymcabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

