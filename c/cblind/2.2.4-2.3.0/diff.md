# Comparing `tmp/cblind-2.2.4.tar.gz` & `tmp/cblind-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wafflarg/cblind/dist/.tmp-r19432cn/cblind-2.2.4.tar", last modified: Wed May 24 10:40:27 2023, max compression
+gzip compressed data, was "/home/wafflarg/cblind/dist/.tmp-ftzpmct0/cblind-2.3.0.tar", last modified: Mon Jun 26 18:06:27 2023, max compression
```

## Comparing `cblind-2.2.4.tar` & `cblind-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.870053 cblind-2.2.4/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-02-25 19:20:47.000000 cblind-2.2.4/LICENSE
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5145 2023-05-24 10:40:27.870053 cblind-2.2.4/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     4590 2023-05-24 10:28:42.000000 cblind-2.2.4/README.md
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.866053 cblind-2.2.4/cblind/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      264 2023-05-24 10:25:37.000000 cblind-2.2.4/cblind/__init__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-05-24 10:28:36.000000 cblind-2.2.4/cblind/__version__.py
--rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)    26291 2023-05-24 10:28:22.000000 cblind-2.2.4/cblind/cblind.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.866053 cblind-2.2.4/cblind.egg-info/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5145 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      506 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/SOURCES.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/dependency_links.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       48 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/entry_points.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       47 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/requires.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        7 2023-05-24 10:40:27.000000 cblind-2.2.4/cblind.egg-info/top_level.txt
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-05-24 10:40:27.870053 cblind-2.2.4/imgs/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    12412 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/bird.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17820 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/cblind.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20566 2021-11-30 15:53:40.000000 cblind-2.2.4/imgs/colormaps.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      619 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/colormaps.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     9126 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/contrast.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    26606 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/extreme_rainbow.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    49866 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/huescale.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1454 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/huescale.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    23133 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/monocolor.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    12215 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/pregunta.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17609 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/rainbow.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    15675 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/rbscale.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    15832 2021-12-01 14:02:06.000000 cblind-2.2.4/imgs/solstice.png
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1009 2023-05-24 10:36:38.000000 cblind-2.2.4/pyproject.toml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-05-24 10:40:27.870053 cblind-2.2.4/setup.cfg
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-26 18:06:27.741580 cblind-2.3.0/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-02-25 19:20:47.000000 cblind-2.3.0/LICENSE
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5163 2023-06-26 18:06:27.741580 cblind-2.3.0/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     4608 2023-06-26 18:02:41.000000 cblind-2.3.0/README.md
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-26 18:06:27.737580 cblind-2.3.0/cblind/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      395 2023-06-26 16:16:09.000000 cblind-2.3.0/cblind/__init__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-06-26 18:02:41.000000 cblind-2.3.0/cblind/__version__.py
+-rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)    28549 2023-06-26 16:16:09.000000 cblind-2.3.0/cblind/cblind.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-26 18:06:27.737580 cblind-2.3.0/cblind.egg-info/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5163 2023-06-26 18:06:27.000000 cblind-2.3.0/cblind.egg-info/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      506 2023-06-26 18:06:27.000000 cblind-2.3.0/cblind.egg-info/SOURCES.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-06-26 18:06:27.000000 cblind-2.3.0/cblind.egg-info/dependency_links.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       48 2023-06-26 18:06:27.000000 cblind-2.3.0/cblind.egg-info/entry_points.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       48 2023-06-26 18:06:27.000000 cblind-2.3.0/cblind.egg-info/requires.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        7 2023-06-26 18:06:27.000000 cblind-2.3.0/cblind.egg-info/top_level.txt
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-26 18:06:27.741580 cblind-2.3.0/imgs/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    12412 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/bird.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17820 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/cblind.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20566 2021-11-30 15:53:40.000000 cblind-2.3.0/imgs/colormaps.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      619 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/colormaps.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     9126 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/contrast.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    26606 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/extreme_rainbow.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    49866 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/huescale.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1454 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/huescale.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    23133 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/monocolor.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    12215 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/pregunta.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17609 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/rainbow.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    15675 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/rbscale.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    15832 2021-12-01 14:02:06.000000 cblind-2.3.0/imgs/solstice.png
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1086 2023-06-26 16:16:09.000000 cblind-2.3.0/pyproject.toml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-06-26 18:06:27.741580 cblind-2.3.0/setup.cfg
```

### Comparing `cblind-2.2.4/LICENSE` & `cblind-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/PKG-INFO` & `cblind-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cblind
-Version: 2.2.4
+Version: 2.3.0
 Summary: Color schemes for Python plots, from Paul Tol (2012)
 Author: G. Wafflard-Fernandez
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/cblind
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,16 +16,16 @@
 
 # cblind
 [![PyPI](https://img.shields.io/pypi/v/cblind)](https://pypi.org/project/cblind/)
 
 A colorblind-friendly python module that allows color choice for plotting multiple curves  
 Works only with python 3  
 8 colormaps are now available to map 2D fields  
-Version: 2.2.4
-Author: Gaylor Wafflard-Fernandez  
+Version: 2.3.0
+Authors: Gaylor Wafflard-Fernandez, Clément Robert  
 Author-email: gaylor.wafflard@univ-grenoble-alpes.fr
 
 ## Installation
 
 Install with `pip`
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cblind-2.2.4/README.md` & `cblind-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # cblind
 [![PyPI](https://img.shields.io/pypi/v/cblind)](https://pypi.org/project/cblind/)
 
 A colorblind-friendly python module that allows color choice for plotting multiple curves  
 Works only with python 3  
 8 colormaps are now available to map 2D fields  
-Version: 2.2.4
-Author: Gaylor Wafflard-Fernandez  
+Version: 2.3.0
+Authors: Gaylor Wafflard-Fernandez, Clément Robert  
 Author-email: gaylor.wafflard@univ-grenoble-alpes.fr
 
 ## Installation
 
 Install with `pip`
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cblind-2.2.4/cblind/cblind.py` & `cblind-2.3.0/cblind/cblind.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import sys
+from math import erf
+from warnings import warn
+
 from cycler import cycler
 
 import numpy as np
-import scipy.special as ss
-import matplotlib.pyplot as plt
+import matplotlib as mpl
 from matplotlib import colors as mcolors
+from matplotlib import colormaps as mcm
 
-from rich import print as rprint
 
 PALETTES = ("cb.rbscale", "cb.rainbow", "cb.huescale", "cb.solstice", "cb.bird", "cb.pregunta", "cb.iris", "cb.extreme_rainbow")
 PALETTES_FULL = (*PALETTES,*tuple([i+"_r" for i in PALETTES]))
 
 STYLES = {
     "solid" : (0, ()),
     "dashed" : (0, (5, 5)),
@@ -95,60 +96,58 @@
     '#DA2222', 
     '#B8221E', 
     '#95211B', 
     '#721E17', 
     '#521A13',
 )
 
-def print_warn(message):
-    """
-    adapted from idefix_cli (cmt robert)
-    https://github.com/neutrinoceros/idefix_cli
-    """
-    rprint(f":eyes: [bold red]Warning[/] {message}", file=sys.stderr)
 
 class Colorplots:
-    def cblind(self, ncurves):
+    def cblind(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle = plt.rcParams['axes.prop_cycle']
+        prop_cycle = mpl.rcParams['axes.prop_cycle']
         clist = prop_cycle.by_key()['color']
         if(ncurves<=4):
             colorscheme = ['#4477AA','#CC6677','#DDCC77','#117733']
         elif(ncurves>4 and ncurves<=12):
             colorscheme = ['#332288','#88CCEE','#117733','#DDCC77','#CC6677','#AA4499','#44AA99','#999933','#882255','#661100','#6699CC','#AA4466']
         elif(ncurves>12 and ncurves<=156):
             colorscheme = ['#332288','#88CCEE','#117733','#DDCC77','#CC6677','#AA4499','#44AA99','#999933','#882255','#661100','#6699CC','#AA4466']
-            print_warn("out of range [1-12]: changed the linestyle")
+            warn("out of range [1-12]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [1-156]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-156]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def contrast(self, ncurves):
+    def contrast(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
-        prop_cycle = plt.rcParams['axes.prop_cycle']
+        prop_cycle = mpl.rcParams['axes.prop_cycle']
         clist = prop_cycle.by_key()['color']
         if(ncurves<=4):
             colorscheme = ['#000000','#004488','#BB5566','#DDAA33']
         elif(ncurves>4 and ncurves<=52):
             colorscheme = ['#000000','#004488','#BB5566','#DDAA33']
-            print_warn("out of range [1-4]: changed the linestyle")
+            warn("out of range [1-4]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [1-52]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-52]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def huescale(self, ncurves, *args):
+    def huescale(self, ncurves, *args, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
         #SET DEFAULT VALUES IF NO OPTIONAL ARGUMENT
-        prop_cycle = plt.rcParams['axes.prop_cycle']
+        prop_cycle = mpl.rcParams['axes.prop_cycle']
         clist = prop_cycle.by_key()['color']
         hue = "None"
         #OPTIONS
         possible_args = ("blue", "bluegreen", "green", "gold", "brown", "rose", "purple")
         for arg in args:
             if arg in possible_args:
                 hue = arg
@@ -170,15 +169,15 @@
                 colorscheme = ['#774411','#AA7744','#DDAA77']
             if hue=='rose':
                 colorscheme = ['#771122','#AA4455','#DD7788']
             if hue=='purple':
                 colorscheme = ['#771155','#AA4488','#CC99BB']
             if hue=='None':
                 colorscheme = ['#D95F0E','#FEC44F','#FFF7BC']
-            plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
 
 
         if(ncurves==4):
             colorscheme = ['#CC4C02','#FB9A29','#FED98E','#FFFBD5']
         if(ncurves==5):
             colorscheme = ['#993404','#D95F0E','#FB9A29','#FED98E','#FFFBD5']
         if(ncurves==6):
@@ -186,25 +185,27 @@
         if(ncurves==7):
             colorscheme = ['#8C2D04','#CC4C02','#EC7014','#FB9A29','#FEC44F','#FEE391','#FFFBD5']
         if(ncurves==8):
             colorscheme = ['#8C2D04','#CC4C02','#EC7014','#FB9A29','#FEC44F','#FEE391','#FFF7BC','#FFFFE5']
         if(ncurves==9):
             colorscheme = ['#662506','#993404','#CC4C02','#EC7014','#FB9A29','#FEC44F','#FEE391','#FFF7BC','#FFFFE5']
         if(ncurves>3 and ncurves<=9 and hue!='None'):
-            print_warn("only ocherscale for more than 3 plots")
+            warn("only ocherscale for more than 3 plots", stacklevel=2)
         if(ncurves>9):
             colorscheme = clist
-            print_warn("out of range [1-9]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-9]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def rbscale(self, ncurves):
+    def rbscale(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle=plt.rcParams['axes.prop_cycle']
+        prop_cycle=mpl.rcParams['axes.prop_cycle']
         clist=prop_cycle.by_key()['color']
 
         if(ncurves==3):
             colorscheme = ['#99C7EC','#FFFAD2','#F5A275']
         elif(ncurves==4):
             colorscheme = ['#008BCE','#B4DDF7','#F9BD7E','#D03232']
         elif(ncurves==5):
@@ -219,25 +220,27 @@
             colorscheme = ['#3A89C9','#77B7E5','#B4DDF7','#E6F5FE','#FFFAD2','#FFE3AA','#F9BD7E','#ED875E','#D24D3E']
         elif(ncurves==10):
             colorscheme = ['#3D52A1','#3A89C9','#77B7E5','#B4DDF7','#E6F5FE','#FFE3AA','#F9BD7E','#ED875E','#D24D3E','#AE1C3E']
         elif(ncurves==11):
             colorscheme = ['#3D52A1','#3A89C9','#77B7E5','#B4DDF7','#E6F5FE','#FFFAD2','#FFE3AA','#F9BD7E','#ED875E','#D24D3E','#AE1C3E']
         elif(ncurves>11 and ncurves<=143):
             colorscheme = ['#3D52A1','#3A89C9','#77B7E5','#B4DDF7','#E6F5FE','#FFFAD2','#FFE3AA','#F9BD7E','#ED875E','#D24D3E','#AE1C3E']
-            print_warn("out of range [3-11]: changed the linestyle")
+            warn("out of range [3-11]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [3-11]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [3-11]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def rainbow(self, ncurves):
+    def rainbow(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle=plt.rcParams['axes.prop_cycle']
+        prop_cycle=mpl.rcParams['axes.prop_cycle']
         clist=prop_cycle.by_key()['color']
 
         if(ncurves==4):
             colorscheme = ['#404096','#57A3AD','#DEA73A','#D92120']
         elif(ncurves==5):
             colorscheme = ['#404096','#529DB7','#7DB874','#E39C37','#D92120']
         elif(ncurves==6):
@@ -252,25 +255,27 @@
             colorscheme = ['#781C81','#3F479B','#4277BD','#529DB7','#62AC9B','#86BB6A','#C7B944','#E39C37','#E76D2E','#D92120']
         elif(ncurves==11):
             colorscheme = ['#781C81','#404096','#416CB7','#4D95BE','#5BA7A7','#6EB387','#A1BE56','#D3B33F','#E59435','#E6682D','#D92120']
         elif(ncurves==12):
             colorscheme = ['#781C81','#413B93','#4065B1','#488BC2','#55A1B1','#63AD99','#7FB972','#B5BD4C','#D9AD3C','#E68E34','#E6642C','#D92120']
         elif(ncurves>12 and ncurves<=156):
             colorscheme = ['#781C81','#413B93','#4065B1','#488BC2','#55A1B1','#63AD99','#7FB972','#B5BD4C','#D9AD3C','#E68E34','#E6642C','#D92120']
-            print_warn("out of range [4-12]: changed the linestyle")
+            warn("out of range [4-12]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [4-12]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [4-12]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def extreme_rainbow(self, ncurves):
+    def extreme_rainbow(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle=plt.rcParams['axes.prop_cycle']
+        prop_cycle=mpl.rcParams['axes.prop_cycle']
         clist=prop_cycle.by_key()['color']
 
         if(ncurves==1):
             colorscheme = [c10]
         elif(ncurves==2):
             colorscheme = [c10,c26]
         elif(ncurves==3):
@@ -315,67 +320,75 @@
             colorscheme = [c2,c4,c5,c7,c8,c9,c10,c11,c13,c14,c15,c16,c17,c18,c19,c21,c23,c25,c26,c27,c28,c29]
         elif(ncurves==23):
             colorscheme = [c1,c2,c4,c5,c7,c8,c9,c10,c11,c13,c14,c15,c16,c17,c18,c19,c21,c23,c25,c26,c27,c28,c29]
         elif(ncurves>23 and ncurves<=34):
             colorscheme = [d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15,d16,d17,d18,d19,d20,d21,d22,d23,d24,d25,d26,d27,d28,d29,d30,d31,d32,d33,d34]
         elif(ncurves>34 and ncurves<=442):
             colorscheme = [d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15,d16,d17,d18,d19,d20,d21,d22,d23,d24,d25,d26,d27,d28,d29,d30,d31,d32,d33,d34]
-            print_warn("out of range [1-34]: changed the linestyle")
+            warn("out of range [1-34]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [1-34]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-34]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def solstice(self, ncurves):
+    def solstice(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle=plt.rcParams['axes.prop_cycle']
+        prop_cycle=mpl.rcParams['axes.prop_cycle']
         clist=prop_cycle.by_key()['color']
         if(ncurves<=11):
             colorscheme = ['#364B9A','#4A7BB7','#6EA6CD','#98CAE1','#C2E4EF','#EAECCC','#FEDA8B','#FDB366','#F67E4B','#DD3D2D','#A50026']
         elif(ncurves>11 and ncurves<=143):
             colorscheme = ['#364B9A','#4A7BB7','#6EA6CD','#98CAE1','#C2E4EF','#EAECCC','#FEDA8B','#FDB366','#F67E4B','#DD3D2D','#A50026']
-            print_warn("out of range [1-11]: changed the linestyle")
+            warn("out of range [1-11]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [1-11]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-11]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def bird(self, ncurves):
+    def bird(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle=plt.rcParams['axes.prop_cycle']
+        prop_cycle=mpl.rcParams['axes.prop_cycle']
         clist=prop_cycle.by_key()['color']
         if(ncurves<=9):
             colorscheme = ['#2166AC','#4393C3','#92C5DE','#D1E5F0','#F7F7F7','#FDDBC7','#F4A582','#D6604D','#B2182B']
         elif(ncurves>9 and ncurves<=117):
             colorscheme = ['#2166AC','#4393C3','#92C5DE','#D1E5F0','#F7F7F7','#FDDBC7','#F4A582','#D6604D','#B2182B']
-            print_warn("out of range [1-9]: changed the linestyle")
+            warn("out of range [1-9]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [1-9]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-9]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
-    def pregunta(self, ncurves):
+    def pregunta(self, ncurves, *, update_prop_cycle=True):
         stylescheme = [STYLES[key] for key in list(STYLES.keys())]
         # stylescheme = [STYLES["solid"]]*ncurves
-        prop_cycle=plt.rcParams['axes.prop_cycle']
+        prop_cycle=mpl.rcParams['axes.prop_cycle']
         clist=prop_cycle.by_key()['color']
         if(ncurves<=9):
             colorscheme = ['#762A83','#9970AB','#C2A5CF','#E7D4E8','#F7F7F7','#D9F0D3','#ACD39E','#5AAE61','#1B7837']
         elif(ncurves>9 and ncurves<=117):
             colorscheme = ['#762A83','#9970AB','#C2A5CF','#E7D4E8','#F7F7F7','#D9F0D3','#ACD39E','#5AAE61','#1B7837']
-            print_warn("out of range [1-9]: changed the linestyle")
+            warn("out of range [1-9]: changed the linestyle", stacklevel=2)
         else:
             colorscheme = clist
-            print_warn("out of range [1-9]: coloblind mode deactivated")
-        plt.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
+            warn("out of range [1-9]: coloblind mode deactivated", stacklevel=2)
+
+        if update_prop_cycle:
+            mpl.rcParams['axes.prop_cycle'] = cycler('linestyle', stylescheme[0:ncurves])*cycler('color', colorscheme[0:ncurves])
         return(colorscheme, stylescheme)
 
     def monocolor(self, ncurves, *args):
         possible_args = ("b&w", "blue", "red", "yellow", "green", "purple")
         printing = "b&w"
         for arg in args:
             if arg in possible_args:
@@ -411,22 +424,28 @@
                 STYLES["densely_dashdotdotted"], 
                 STYLES["loosely_dashed"], 
                 STYLES["loosely_dotted"], 
                 STYLES["loosely_dashdotted"], 
                 STYLES["loosely_dashdotdotted"],
             ]
             if(ncurves>13):
-                print_warn("maximum 13 different linestyles")
+                warn("maximum 13 different linestyles", stacklevel=2)
                 stylescheme = stylescheme*int(np.ceil(ncurves/13))
             stylescheme = stylescheme[0:ncurves]
             default_cycler=(cycler(color=colorscheme)+cycler(linestyle=stylescheme))
-            plt.rc('axes', prop_cycle=default_cycler)
+            mpl.rc('axes', prop_cycle=default_cycler)
         return(colorscheme,stylescheme)
 
 def reversed_cmap(cmap, name = 'my_cmap_r', nbin=None):
+    warn(
+        "cblind.reversed_cmap(cm, ...) is deprecated. "
+        "Please use cm.reversed() instead. ",
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
     if nbin is None:
         nbin=256
     reverse = []                  
     k = []                          
 
     for key in cmap._segmentdata:    
         k.append(key)
@@ -436,17 +455,35 @@
             data.append((1-t[0],t[2],t[1]))            
         reverse.append(sorted(data))    
 
     LinearL = dict(zip(k,reverse))
     my_cmap_r = mcolors.LinearSegmentedColormap(name, LinearL, N=nbin) 
     return my_cmap_r
 
-def _get_cbmap(palette, nbin=None):
-    if nbin is None:
-        nbin=256
+
+_REGISTERED = set()
+def _register_to_mpl(name):
+    if name in _REGISTERED:
+        return
+    cbcmap = _get_cbmap(name)
+
+    mcm.register(cbcmap)
+    mcm.register(cbcmap.reversed())
+    _REGISTERED.add(name)
+
+def _erf_vector(arr):
+    # a simple substitute for scipy.special.erf
+    # performance is about 1/20 with respect to scipy impl
+    # but results are still obtained within well below 1ms for 256 elements
+    # which is the typical application
+    out = np.empty_like(arr)
+    out[:] = [erf(_) for _ in arr]
+    return out
+
+def _get_cbmap(palette, nbin=256):
     x=np.linspace(0.,1.,nbin)
     if palette not in PALETTES_FULL:
         raise NotImplementedError(
             f"palette '{palette}' not implemented yet in _get_cbmap function"
         )
     palette_tmp = palette
     if palette[-2:]=="_r":
@@ -457,59 +494,81 @@
         green=((0.572+1.524*x-1.811*x**2)/(1.-0.291*x+0.1574*x**2))**2
         blue=(1./(1.579-4.03*x+12.92*x**2-31.4*x**3+48.6*x**4-23.36*x**5))
     elif palette_tmp=='cb.rainbow':
         red = (0.472-0.567*x+4.05*x**2)/(1.+8.72*x-19.17*x**2+14.1*x**3)
         green = 0.108932-1.22635*x+27.284*x**2-98.577*x**3+163.3*x**4-131.395*x**5+40.634*x**6
         blue = 1./(1.97+3.54*x-68.5*x**2+243*x**3-297*x**4+125*x**5)
     elif palette_tmp=='cb.huescale':
-        red = 1.-0.392*(1.+ss.erf((x-0.869)/0.255))
-        green = 1.021-0.456*(1.+ss.erf((x-0.527)/0.376))
-        blue = 1.-0.493*(1.+ss.erf((x-0.272)/0.309))
+        red = 1.-0.392*(1.+_erf_vector((x-0.869)/0.255))
+        green = 1.021-0.456*(1.+_erf_vector((x-0.527)/0.376))
+        blue = 1.-0.493*(1.+_erf_vector((x-0.272)/0.309))
 
     if palette_tmp=="cb.rbscale" or palette_tmp=="cb.rainbow" or palette_tmp=="cb.huescale":
-        redline=[]
-        greenline=[]
-        blueline=[]
-        for i in range(len(x)):
-            redline.append((x[i],red[i],red[i]))
-            greenline.append((x[i],green[i],green[i]))
-            blueline.append((x[i],blue[i],blue[i]))
+        redline = np.empty((len(x), 3))
+        greenline = np.empty((len(x), 3))
+        blueline = np.empty((len(x), 3))
+
+        redline[:, 0] = greenline[:, 0] = blueline[:, 0] = x
+        redline[:, 1] = redline[:, 2] = red
+        greenline[:, 1] = greenline[:, 2] = green
+        blueline[:, 1] = blueline[:, 2] = blue
 
         cdict = {'red':   redline,
                  'green': greenline,
                  'blue': blueline}
 
         cbcmap = mcolors.LinearSegmentedColormap(f"{palette_tmp}", cdict, N=nbin)
     elif palette_tmp=="cb.extreme_rainbow":
-        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().extreme_rainbow(34)[0], N=nbin)
+        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().extreme_rainbow(34, update_prop_cycle=False)[0], N=nbin)
     elif palette_tmp=="cb.solstice":
-        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().solstice(11)[0], N=nbin)
+        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().solstice(11, update_prop_cycle=False)[0], N=nbin)
     elif palette_tmp=="cb.bird":
-        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().bird(9)[0], N=nbin)
+        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().bird(9, update_prop_cycle=False)[0], N=nbin)
     elif palette_tmp=="cb.pregunta":
-        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().pregunta(9)[0], N=nbin)
+        cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", Colorplots().pregunta(9, update_prop_cycle=False)[0], N=nbin)
     elif palette_tmp=="cb.iris":
         cmap_iris = ["#FEFBE9", "#FCF7D5", "#F5F3C1", "#EAF0B5", "#DDECBF", "#D0E7CA", "#C2E3D2", "#B5DDD8", "#A8D8DC", "#9BD2E1", "#8DCBE4", "#81C4E7", "#7BBCE7", "#7EB2E4", "#88A5DD", "#9398D2", "#9B8AC4", "#9D7DB2", "#9A709E", "#906388", "#805770", "#684957", "#46353A"]
         cbcmap = mcolors.LinearSegmentedColormap.from_list(f"{palette_tmp}", cmap_iris, N=nbin)
     if palette[-2:]=="_r":
-        cbcmap = reversed_cmap(cbcmap, name=f"{palette}_r", nbin=nbin)
+        cbcmap = cbcmap.reversed()
     return(cbcmap)
 
 def cbmap(palette=None, nbin=None):
+    warn(
+        "cblind.cbmap is deprecated. "
+        "Please use matplotlib.colormaps.get_cmap instead, or "
+        "matplotlib.pyplot.get_cmap if you need to specify nbin "
+        "(default is 256)",
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
     if palette not in PALETTES_FULL:
-        palette = plt.get_cmap(palette, nbin)
+        if nbin is None:
+            return mcm.get_cmap(palette)
+        else:
+            import matplotlib.pyplot as plt
+
+            return plt.get_cmap(palette, nbin)
     else:
-        palette = _get_cbmap(palette, nbin)
-    return palette
+        return _get_cbmap(palette, nbin)
 
 def mapping(fig, ax, data2d, palette=None, nbin=None):
-    im=ax.imshow(data2d, cmap=cbmap(palette=palette, nbin=nbin), aspect='auto')
+    if nbin is None:
+        cmap = mcm.get_cmap(palette)
+    else:
+        import matplotlib.pyplot as plt
+
+        cmap = plt.get_cmap(palette, nbin)
+    
+    im=ax.imshow(data2d, cmap=cmap, aspect='auto')
     fig.colorbar(im)
 
 def test_cblind(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().cblind(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -517,14 +576,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=1.5)
 
     plt.show()
 
 def test_contrast(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().contrast(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -532,14 +593,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=1.5)
 
     plt.show()
 
 def test_huescale(ny, *args):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().huescale(ny, *args)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -547,14 +610,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_rbscale(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().rbscale(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -562,14 +627,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_solstice(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().solstice(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -577,14 +644,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_bird(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().bird(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -592,14 +661,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_pregunta(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().pregunta(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -607,14 +678,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_rainbow(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().rainbow(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -622,14 +695,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_extreme_rainbow(ny):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().extreme_rainbow(ny)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -637,14 +712,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=2.0)
 
     plt.show()
 
 def test_monocolor(ny, *args):
+    import matplotlib.pyplot as plt
+
     nx=100
     x=np.linspace(0,10, nx)
     y=np.zeros((ny,nx), dtype=int)
     color, linestyle = Colorplots().monocolor(ny, *args)
 
     fig, ax = plt.subplots()
     for i in range(ny):
@@ -652,14 +729,16 @@
             y[i][j]=x[j]+i
         # plt.plot(x,y[i], color[i], linewidth=2.0)
         ax.plot(x,y[i], linewidth=1.0)
 
     plt.show()
 
 def test_mapping(palette=None,nbin=None):
+    import matplotlib.pyplot as plt
+
     fig, ax = plt.subplots()
 
     r = np.arange(-np.pi, np.pi, 0.1)
     t = np.arange(0, 2*np.pi, 0.1)
     X, Y = np.meshgrid(r, t)
     data = np.cos(X) * np.sin(Y) * 10
```

### Comparing `cblind-2.2.4/cblind.egg-info/PKG-INFO` & `cblind-2.3.0/cblind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cblind
-Version: 2.2.4
+Version: 2.3.0
 Summary: Color schemes for Python plots, from Paul Tol (2012)
 Author: G. Wafflard-Fernandez
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/cblind
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,16 +16,16 @@
 
 # cblind
 [![PyPI](https://img.shields.io/pypi/v/cblind)](https://pypi.org/project/cblind/)
 
 A colorblind-friendly python module that allows color choice for plotting multiple curves  
 Works only with python 3  
 8 colormaps are now available to map 2D fields  
-Version: 2.2.4
-Author: Gaylor Wafflard-Fernandez  
+Version: 2.3.0
+Authors: Gaylor Wafflard-Fernandez, Clément Robert  
 Author-email: gaylor.wafflard@univ-grenoble-alpes.fr
 
 ## Installation
 
 Install with `pip`
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cblind-2.2.4/imgs/bird.png` & `cblind-2.3.0/imgs/bird.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/cblind.png` & `cblind-2.3.0/imgs/cblind.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/colormaps.png` & `cblind-2.3.0/imgs/colormaps.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/colormaps.py` & `cblind-2.3.0/imgs/colormaps.py`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/contrast.png` & `cblind-2.3.0/imgs/contrast.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/extreme_rainbow.png` & `cblind-2.3.0/imgs/extreme_rainbow.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/huescale.png` & `cblind-2.3.0/imgs/huescale.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/huescale.py` & `cblind-2.3.0/imgs/huescale.py`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/monocolor.png` & `cblind-2.3.0/imgs/monocolor.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/pregunta.png` & `cblind-2.3.0/imgs/pregunta.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/rainbow.png` & `cblind-2.3.0/imgs/rainbow.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/rbscale.png` & `cblind-2.3.0/imgs/rbscale.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/imgs/solstice.png` & `cblind-2.3.0/imgs/solstice.png`

 * *Files identical despite different names*

### Comparing `cblind-2.2.4/pyproject.toml` & `cblind-2.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cblind"
-version = "2.2.4"
 description = "Color schemes for Python plots, from Paul Tol (2012)"
 authors = [
     { name = "G. Wafflard-Fernandez" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
 ]
 requires-python = ">=3.6"
 dependencies = [
-    "matplotlib",
+    "matplotlib>=3.5",
+    "cycler",
     "numpy",
-    "rich",
-    "scipy",
 ]
+dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.license]
 text = "GPL-3.0"
@@ -47,7 +46,10 @@
 license-files = [
     "LICENSE",
 ]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 namespaces = false
+
+[tool.setuptools.dynamic]
+version = {attr = "cblind.__version__.__version__"}
```

