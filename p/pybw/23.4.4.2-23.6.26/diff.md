# Comparing `tmp/pybw-23.4.4.2.tar.gz` & `tmp/pybw-23.6.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybw-23.4.4.2.tar", last modified: Tue Apr  4 04:44:23 2023, max compression
+gzip compressed data, was "pybw-23.6.26.tar", last modified: Mon Jun 26 16:13:04 2023, max compression
```

## Comparing `pybw-23.4.4.2.tar` & `pybw-23.6.26.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.636054 pybw-23.4.4.2/
--rw-rw-rw-   0        0        0      577 2023-04-03 07:29:43.000000 pybw-23.4.4.2/- command.txt
--rw-rw-rw-   0        0        0     1187 2023-03-14 02:03:31.000000 pybw-23.4.4.2/LICENSE
--rw-rw-rw-   0        0        0       17 2023-03-14 02:03:31.000000 pybw-23.4.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      732 2023-04-04 04:44:23.634068 pybw-23.4.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-03-14 02:03:31.000000 pybw-23.4.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.566055 pybw-23.4.4.2/pybw/
--rw-rw-rw-   0        0        0        0 2023-03-14 02:03:31.000000 pybw-23.4.4.2/pybw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.579070 pybw-23.4.4.2/pybw/ccnb_mod/
--rw-rw-rw-   0        0        0        0 2023-03-14 02:03:31.000000 pybw-23.4.4.2/pybw/ccnb_mod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.602054 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/
--rw-rw-rw-   0        0        0    21496 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysis.py
--rw-rw-rw-   0        0        0    23935 2022-08-21 14:07:41.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py
--rw-rw-rw-   0        0        0     5071 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVSEParam.dat
--rw-rw-rw-   0        0        0    24461 2022-08-18 06:43:45.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/Structure.py
--rw-rw-rw-   0        0        0     8889 2022-08-21 07:59:31.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.623057 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/
--rw-rw-rw-   0        0        0    14330 2022-08-11 03:54:41.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
--rw-rw-rw-   0        0        0    15658 2022-08-21 14:07:58.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
--rw-rw-rw-   0        0        0    22032 2022-08-21 07:46:04.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
--rw-rw-rw-   0        0        0     8727 2022-08-21 07:59:41.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    43144 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvmparam.dat
--rw-rw-rw-   0        0        0    31000 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvse.dat
--rw-rw-rw-   0        0        0     6500 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/elements.dat
--rw-rw-rw-   0        0        0     7538 2022-08-18 08:53:58.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/temp.py
--rw-rw-rw-   0        0        0    17720 2023-03-16 06:53:29.000000 pybw-23.4.4.2/pybw/ccnb_mod/ccnb_mod.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.625052 pybw-23.4.4.2/pybw/core/
--rw-rw-rw-   0        0        0     2361 2023-04-04 04:43:57.000000 pybw-23.4.4.2/pybw/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.629071 pybw-23.4.4.2/pybw/tricks/
--rw-rw-rw-   0        0        0      119 2023-03-14 02:03:31.000000 pybw-23.4.4.2/pybw/tricks/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-04-04 02:31:30.000000 pybw-23.4.4.2/pybw/tricks/lazy_import.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.544056 pybw-23.4.4.2/pybw/utils/
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.631068 pybw-23.4.4.2/pybw/utils/pymatgen/
--rw-rw-rw-   0        0        0     7582 2023-03-14 08:29:49.000000 pybw-23.4.4.2/pybw/utils/pymatgen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.575053 pybw-23.4.4.2/pybw.egg-info/
--rw-rw-rw-   0        0        0      732 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       17 2023-03-14 02:03:31.000000 pybw-23.4.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 04:44:23.636054 pybw-23.4.4.2/setup.cfg
--rw-rw-rw-   0        0        0     3051 2023-04-04 04:44:14.000000 pybw-23.4.4.2/setup.py
--rwxrwxrwx   0        0        0      221 2023-04-03 07:29:43.000000 pybw-23.4.4.2/upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.083360 pybw-23.6.26/
+-rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw-23.6.26/- command.txt
+-rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw-23.6.26/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw-23.6.26/MANIFEST.in
+-rw-rw-rw-   0        0        0      754 2023-06-26 16:13:04.081359 pybw-23.6.26/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-03-13 12:06:00.000000 pybw-23.6.26/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.901716 pybw-23.6.26/pybw/
+-rw-rw-rw-   0        0        0        0 2023-03-13 14:57:12.000000 pybw-23.6.26/pybw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.952348 pybw-23.6.26/pybw/ccnb_mod/
+-rw-rw-rw-   0        0        0        0 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.011352 pybw-23.6.26/pybw/ccnb_mod/bvseLi/
+-rw-rw-rw-   0        0        0    22034 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysis.py
+-rw-rw-rw-   0        0        0    24506 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py
+-rw-rw-rw-   0        0        0     5071 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVSEParam.dat
+-rw-rw-rw-   0        0        0    25155 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/Structure.py
+-rw-rw-rw-   0        0        0     9177 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.037354 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/
+-rw-rw-rw-   0        0        0    14330 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    15658 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
+-rw-rw-rw-   0        0        0    22032 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8727 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    45065 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvmparam.dat
+-rw-rw-rw-   0        0        0    31592 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvse.dat
+-rw-rw-rw-   0        0        0     6681 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/elements.dat
+-rw-rw-rw-   0        0        0     7678 2023-04-04 04:49:42.000000 pybw-23.6.26/pybw/ccnb_mod/bvseLi/temp.py
+-rw-rw-rw-   0        0        0    17720 2023-03-18 14:08:38.000000 pybw-23.6.26/pybw/ccnb_mod/ccnb_mod.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.043356 pybw-23.6.26/pybw/core/
+-rw-rw-rw-   0        0        0     2551 2023-06-26 15:51:36.000000 pybw-23.6.26/pybw/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.051356 pybw-23.6.26/pybw/scholar/
+-rw-rw-rw-   0        0        0     1714 2023-04-10 07:40:49.000000 pybw-23.6.26/pybw/scholar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.066357 pybw-23.6.26/pybw/tricks/
+-rw-rw-rw-   0        0        0      114 2023-06-26 15:52:27.000000 pybw-23.6.26/pybw/tricks/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-06-26 15:54:12.000000 pybw-23.6.26/pybw/tricks/lazy_import.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.837711 pybw-23.6.26/pybw/utils/
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:04.073358 pybw-23.6.26/pybw/utils/pymatgen/
+-rw-rw-rw-   0        0        0     7582 2023-03-14 13:35:46.000000 pybw-23.6.26/pybw/utils/pymatgen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:13:03.937347 pybw-23.6.26/pybw.egg-info/
+-rw-rw-rw-   0        0        0      754 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 16:13:03.000000 pybw-23.6.26/pybw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       15 2023-03-13 12:06:00.000000 pybw-23.6.26/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:13:04.083360 pybw-23.6.26/setup.cfg
+-rw-rw-rw-   0        0        0     3052 2023-06-26 16:01:11.000000 pybw-23.6.26/setup.py
+-rwxrwxrwx   0        0        0      357 2023-06-26 16:12:48.000000 pybw-23.6.26/upload_pypi.bat
```

### Comparing `pybw-23.4.4.2/- command.txt` & `pybw-23.6.26/- command.txt`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/LICENSE` & `pybw-23.6.26/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-Copyright (c) 2011-2012 MIT & The Regents of the University of California,
-through Lawrence Berkeley National Laboratory
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+Copyright (c) 2011-2012 MIT & The Regents of the University of California,
+through Lawrence Berkeley National Laboratory
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pybw-23.4.4.2/PKG-INFO` & `pybw-23.6.26/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: pybw
-Version: 23.4.4.2
+Version: 23.6.26
 Summary: pybw
 Home-page: https://gitee.com/pubowei/pybw
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/pybw
 Project-URL: Package, https://pypi.org/project/pybw
 Project-URL: Repo, https://gitee.com/pubowei/pybw
 Keywords: pybw,tools
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pybw
 
 Some convenient useful tools
 
+
+
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysis.py` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysis.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,538 +1,538 @@
-'''
-Created on 2017
-
-@author: hebing
-'''
-import os
-import numpy as np
-from scipy.special import erfc
-from scipy.ndimage import measurements
-import scipy.ndimage
-import math
-from struct import pack
-
-
-def loadbvparam(filename):
-    with open(filename, 'r') as fp:
-        lines = fp.readlines()
-    bvmpara = {}
-    for line in lines:
-        varstr = line.split('\t')
-        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
-        if key in bvmpara:
-            bvmpara[key].append([float(varstr[4]), float(varstr[5])])
-        else:
-            bvmpara[key] = [[float(varstr[4]), float(varstr[5])]]
-    return bvmpara
-
-
-def loadBVSEparam(filename):
-    with open(filename, 'r') as fp:
-        lines = fp.readlines()
-    BVSEparam = {}
-    for line in lines[1:]:
-        line = line.strip('\n')
-        varstr = line.split('\t')
-        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
-        if key in BVSEparam:
-            BVSEparam[key].append([
-                float(varstr[4]),
-                float(varstr[5]),
-                float(varstr[6]),
-                float(varstr[7]),
-                float(varstr[8]),
-                float(varstr[9])
-            ])
-        else:
-            BVSEparam[key] = [[
-                float(varstr[4]),
-                float(varstr[5]),
-                float(varstr[6]),
-                float(varstr[7]),
-                float(varstr[8]),
-                float(varstr[9])
-            ]]
-    return BVSEparam
-
-
-def loadElementsparam(filename):
-    with open(filename, 'r') as fp:
-        lines = fp.readlines()
-    Elementsparam = {}
-    for line in lines:
-        line = line.strip('\n')
-        varstr = line.split('\t')
-        key = varstr[1] + varstr[2]
-        Elementsparam[key] = [
-            float(varstr[0]),
-            float(varstr[3]),
-            float(varstr[4]),
-            float(varstr[5]),
-            float(varstr[6]),
-            float(varstr[7]),
-            float(varstr[8]),
-            float(varstr[9])
-        ]
-    return Elementsparam
-
-
-class BVAnalysis(object):
-    '''
-    for bond valence method analyze ion channel
-    '''
-
-    def __init__(self, struc=None, size=[50, 50, 50]):
-        '''
-        Constructor
-        '''
-        self._Struct = struc
-        self._Size = [50, 50, 50]
-        self.__Data = {}
-        self.__Max = {}
-        self.__Min = {}
-        self.Ea = {}
-        self._MoveIon = 'Li'
-        self._poss = None
-        self.ValenceOfMoveIon = 1
-        self.stop = False
-        module_dir = os.path.dirname(os.path.abspath(__file__))
-
-        self._BVparam = loadbvparam(os.path.join(module_dir, 'bvmparam.dat'))
-        self._BVSEparam = loadBVSEparam(os.path.join(module_dir, 'bvse.dat'))
-        self._Elementsparam = loadElementsparam(
-            os.path.join(module_dir, 'elements.dat'))
-
-    def get_data(self):
-        return self.__Data
-
-    def get_max(self):
-        return self.__Max
-
-    def get_min(self):
-        return self.__Min
-
-    def set_data(self, value):
-        self.__Data = value
-
-    def set_max(self, value):
-        self.__Max = value
-
-    def set_min(self, value):
-        self.__Min = value
-
-    def del_data(self):
-        del self.__Data
-
-    def del_max(self):
-        del self.__Max
-
-    def del_min(self):
-        del self.__Min
-
-    @property
-    def BVSMin(self):
-        return self.__Min['BVS']
-
-    @property
-    def BVSEMin(self):
-        return self.__Min['BVSE']
-
-    @property
-    def BVELMin(self):
-        return self.__Min['BVEL']
-
-    @property
-    def BVSMax(self):
-        return self.__Max['BVS']
-
-    @property
-    def BVSEMax(self):
-        return self.__Max['BVSE']
-
-    @property
-    def BVELMax(self):
-        return self.__Max['BVEL']
-
-    @property
-    def BVSEEa(self):
-        return self.Ea['BVSE']
-
-    @property
-    def BVELEa(self):
-        return self.Ea['BVEL']
-
-    def SetStructure(self, struc):
-        self._Struct = struc
-
-    def SetMoveIon(self, moveion):
-        self._MoveIon = moveion
-
-    def SetResolution(self, size):
-        self._Size = size
-
-    def SetLengthResolution(self, reslen=0.1):
-        abc = self._Struct.Getabc()
-        self._reslen = reslen
-        self._Size[0] = int(abc[0] / reslen) + 1
-        self._Size[1] = int(abc[1] / reslen) + 1
-        self._Size[2] = int(abc[2] / reslen) + 1
-
-    def SaveBVSEData(self, filename):
-        self.SaveBinaryData(filename + '_BVSE.pgrid', self.__Data['BVSE'],
-                            'BVSE')
-        np.save(filename + "_BVSE.npy", self.__Data['BVSE'])
-
-    def SaveBVELData(self, filename):
-        self.SaveBinaryData(filename + '_BVEL.pgrid', self.__Data['BVEL'],
-                            'BVEL')
-
-    def SaveBVSData(self, filename):
-        self.SaveBinaryData(filename + '_BVS.pgrid', self.__Data['BVS'], 'BVS')
-
-    def SaveData(self, filename, data, datatype=' '):
-        fp = open(filename, 'w')
-        fp.write(datatype + '\n')
-        alpha = self._Struct.GetAlphaBetaGama()
-        abc = self._Struct.Getabc()
-        fp.write(str(abc[0]) + ' ' + str(abc[1]) + ' ' + str(abc[2]) + ' ')
-        fp.write(
-            str(alpha[0]) + ' ' + str(alpha[1]) + ' ' + str(alpha[2]) + '\n')
-        fp.write(
-            str(self._Size[0]) + ' ' + str(self._Size[1]) + ' ' +
-            str(self._Size[2]) + '\n ')
-        for i in range(self._Size[0]):
-            for j in range(self._Size[1]):
-                for k in range(self._Size[2]):
-                    fp.write(str(data[i][j][k]) + '\n')
-        fp.close()
-
-    def SaveBinaryData(self, filename, data, datatype=' '):
-        latticeparam = self._Struct.Getabc() + self._Struct.GetAlphaBetaGama()
-        with open(filename, 'wb') as outf:
-            outf.write(pack('4i', 3, 0, 0, 0))  # file format version
-            outf.write(pack(
-                '80s',
-                datatype.ljust(80).encode('utf-8')))  # Title 80 characters
-            outf.write(pack('i', 1))  # gType 0 for *.ggrid, 1 for *.pgrid
-            outf.write(pack('i', 0))  # fType 0
-            outf.write(pack('i', 1))  # nVal dummy
-            outf.write(pack('i', 3))  # dimension
-            outf.write(pack('3i', *self._Size))  # numbers of voxels
-            outf.write(pack('i', data.size))  # Total number of voxels
-            outf.write(pack('6f', *latticeparam))  # lattice parameters
-            for k in range(self._Size[2]):
-                for j in range(self._Size[1]):
-                    for i in range(self._Size[0]):
-                        outf.write(pack('f', data[i][j][k]))
-
-    def ReadData(self, filename, data, datatype=' '):
-        fp = open(filename, 'r')
-        datatype = fp.readline()
-        alpha = self._Struct.GetAlphaBetaGama()
-        abc = self._Struct.Getabc()
-        abc = fp.readline().split()
-        alpha = fp.readline().split()
-        strs = fp.readline().split()
-        size = [int(i) for i in strs]
-        if datatype == 'bvs':
-            self.__Data['BVS'] = np.zeros(size)
-            data = self.__Data['BVS']
-        else:
-            self.__Data['BVSE'] = np.zeros(size)
-            data = self.__Data['BVSE']
-        for i in range(size[2]):
-            for j in range(size[1]):
-                for k in range(size[0]):
-                    strs = fp.readline().split()
-                    data[k][j][i] = int(strs[0])
-
-        fp.close()
-
-    def GetBVSData(self):
-        return self.__Data['BVS']
-
-    def GetBVSEData(self):
-        return self.__Data['BVSE']
-
-    def GetPosSet(self):
-        return self._poss
-
-    def CaluGlobalIndex(self, ):
-        self.stop = False
-        self._Size.reverse()
-        centrepos = np.zeros(self._Size + [3])
-        self._Data = np.zeros(self._Size, dtype=np.double)
-        for k in range(self._Size[0]):
-            for j in range(self._Size[1]):
-                for i in range(self._Size[2]):
-                    centrepos[k][j][i][2] = k / (self._Size[0] - 1.0)
-                    centrepos[k][j][i][1] = j / (self._Size[1] - 1.0)
-                    centrepos[k][j][i][0] = i / (self._Size[2] - 1.0)
-
-        self._poss = self._Struct.FracPosToCartPos(centrepos)
-        (distance, neighborsindex) = self._Struct.GetKNeighbors(self._poss,
-                                                                kn=8)
-
-        site2atoms = None
-        for k in range(self._Size[0]):
-
-            for j in range(self._Size[1]):
-                for i in range(self._Size[2]):
-                    if self.stop:
-                        return
-                    for dindex, index in enumerate(neighborsindex[k][j][i]):
-                        site2 = self._Struct.GetSuperCellusites()[index]
-                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
-                            for key in site2.GetElementsOccupy():
-                                if key != 'Vac':
-                                    site2atoms = key
-                            if self.ValenceOfMoveIon > 0:
-                                key = "".join([
-                                    self._MoveIon,
-                                    str(self.ValenceOfMoveIon), site2atoms,
-                                    str(site2.GetElementsOxiValue()
-                                        [site2atoms])
-                                ])
-                            else:
-                                key = "".join([
-                                    site2atoms,
-                                    str(site2.GetElementsOxiValue()
-                                        [site2atoms]), self._MoveIon,
-                                    str(self.ValenceOfMoveIon)
-                                ])
-                            if key in self._BVparam:
-                                (r, b) = self._BVparam[key][0]
-                                bv = np.exp(
-                                    (r - distance[k][j][i][dindex]) / b)
-                                self.__Data['BVS'][k][j][
-                                    i] = self.__Data['BVS'][k][j][i] + bv
-                            else:
-                                print('Not Find bvs param' + key)
-                        else:
-                            pass
-                            #print(site2.GetSiteLabel())
-    def CaluBVSE(self, ProgressCall):
-        if len(self._Struct._OxidationTable) == 0:
-            raise Exception(
-                "can't caculation bvs and Ea without atom oxi info !")
-        self.stop = False
-        centrepos = np.zeros(self._Size + [3])
-        self.__Data['BVS'] = np.zeros(self._Size, dtype=np.double)
-        self.__Data['BVSE'] = np.zeros(self._Size, dtype=np.double)
-        self.__Data['BVEL'] = np.zeros(self._Size, dtype=np.double)
-        for k in range(self._Size[2]):
-            for j in range(self._Size[1]):
-                for i in range(self._Size[0]):
-                    centrepos[i][j][k][2] = k / (self._Size[2] - 1.0)
-                    centrepos[i][j][k][1] = j / (self._Size[1] - 1.0)
-                    centrepos[i][j][k][0] = i / (self._Size[0] - 1.0)
-        if ProgressCall:
-            ProgressCall(10)
-        self._poss = self._Struct.FracPosToCartPos(centrepos)
-
-        atomsq = {}
-        for atom in self._Struct._atomsymbols:
-            atomsq[atom] = 0
-            for site in self._Struct._Sites:
-                if atom in site.GetElements():
-                    key = atom + str(site.GetElementsOxiValue()[atom])
-                    atomsq[atom] = atomsq[atom] + site.GetElementsOxiValue(
-                    )[atom] * site.GetElementsOccupy()[atom] / math.sqrt(
-                        self._Elementsparam[key][3])
-        qsumanion = 0
-        qsumcation = 0
-        for (atom, value) in atomsq.items():
-            if value > 0:
-                qsumcation = qsumcation + value
-            elif value < 0:
-                qsumanion = qsumanion + value
-            else:
-                qsumanion = 0
-                qsumcation = 0
-        qsum = 0.0
-        if self.ValenceOfMoveIon > 0:
-            qsum = -qsumanion / qsumcation
-        else:
-            qsum = -qsumcation / qsumanion
-        key1 = self._MoveIon + str(self.ValenceOfMoveIon)
-        qm1 = self.ValenceOfMoveIon / math.sqrt(self._Elementsparam[key1][3])
-        rm1 = self._Elementsparam[key1][6]
-        for i in range(self._Size[0]):
-            (distance,
-             neighborsindex) = self._Struct.GetKNeighbors(self._poss[i],
-                                                          kn=128)
-            if ProgressCall:
-                ProgressCall(10 + i * 90 / (self._Size[0] - 1))
-            for j in range(self._Size[1]):
-                for k in range(self._Size[2]):
-                    if self.stop:
-                        return False
-                    bvsdata = 0.0
-                    data = 0.0
-                    cdata = 0.0
-                    bvelcdata = 0.0
-                    N = 0
-                    D0 = 0.0
-                    Rcutoff = 10.0
-                    alpha = 0.0
-                    occupyvalue = 0.0
-                    for dindex, index in enumerate(neighborsindex[j][k]):
-                        site2 = self._Struct._SuperCellusites[index]
-                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
-                            for (ssymbol, occupyvalue
-                                 ) in site2.GetElementsOccupy().items():
-                                if ssymbol != 'Vac':
-                                    site2oxi = site2.GetElementsOxiValue(
-                                    )[ssymbol]
-                                    if self.ValenceOfMoveIon > 0:
-                                        key = "".join([
-                                            self._MoveIon,
-                                            str(self.ValenceOfMoveIon),
-                                            ssymbol,
-                                            str(site2oxi)
-                                        ])
-                                    else:
-                                        key = "".join([
-                                            ssymbol,
-                                            str(site2oxi), self._MoveIon,
-                                            str(self.ValenceOfMoveIon)
-                                        ])
-                                    if (key in self._BVSEparam) and (
-                                            key in self._BVparam):
-                                        (Nc, r0, Rcutoff, D0, Rmin,
-                                         alpha) = self._BVSEparam[key][0]
-                                        (r, b) = self._BVparam[key][0]
-                                        Rcutoff = 10.0
-                                        if distance[j][k][dindex] <= Rcutoff:
-                                            # bv=np.exp((r0-distance[k][j][i][dindex])*alpha)
-                                            bvs = np.exp(
-                                                (r - distance[j][k][dindex]) /
-                                                b)
-                                            smin = np.exp(
-                                                (Rmin - distance[j][k][dindex])
-                                                * alpha)
-                                            en_s = np.exp(
-                                                (Rmin - Rcutoff) * alpha)
-                                            bvsdata = bvsdata + bvs  #*occupyvalue-((en_s-1)**2-1)
-                                            data = data + ((smin - 1)**2 -
-                                                           1) * occupyvalue
-                                    else:
-                                        if (key not in self._BVSEparam):
-                                            raise Exception(
-                                                "bvse {0}  param can't find!!!!"
-                                                .format(key))
-                                            ProgressCall(0)
-                                        else:
-                                            raise Exception(
-                                                "bvs {0} param can't find!!!!".
-                                                format(key))
-                                            ProgressCall(0)
-                        else:
-                            for (ssymbol, occupyvalue
-                                 ) in site2.GetElementsOccupy().items():
-                                if ssymbol != 'Vac':
-                                    site2oxi = site2.GetElementsOxiValue(
-                                    )[ssymbol]
-                                    if ssymbol != self._MoveIon:
-                                        key = ssymbol + str(site2oxi)
-                                        rm2 = self._Elementsparam[key][6]
-                                        qm2 = site2oxi / math.sqrt(
-                                            self._Elementsparam[key][3])
-                                        rm1m2 = distance[j][k][dindex]
-                                        f = 0.74
-                                        if rm1m2 > rm2:
-                                            if rm1m2 < Rcutoff:
-                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(
-                                                    rm1m2 /
-                                                    (f * (rm1 + rm2))) * qsum
-                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (
-                                                    erfc(rm1m2 /
-                                                         (f * (rm1 + rm2))) -
-                                                    erfc(Rcutoff /
-                                                         (f * (rm1 + rm2))))
-                                        else:
-                                            cdata = 300
-                                            bvelcdata = 300
-                    self.__Data['BVSE'][i][j][k] = (0.5 * D0 * (data) +
-                                                    14.4 * cdata)
-                    self.__Data['BVS'][i][j][k] = bvsdata
-                    self.__Data['BVEL'][i][j][k] = (D0 * (data) +
-                                                    14.4 * bvelcdata)
-        self.__Data['BVSE'] = self.__Data['BVSE']  #/self.ValenceOfMoveIon
-        self.__Data['BVEL'] = self.__Data['BVEL']  #/self.ValenceOfMoveIon
-        for key, data in self.__Data.items():
-            self.__Max[key] = np.max(data)
-            self.__Min[key] = np.min(data)
-            ashape = self.__Data['BVSE'].shape
-            self.ndata = np.zeros(
-                (2 * ashape[0], 2 * ashape[1], 2 * ashape[2]))
-            for i in range(2):
-                for j in range(2):
-                    for k in range(2):
-                        self.ndata[i*ashape[0]:(i+1)*ashape[0], \
-                                                 j*ashape[1]:(j+1)*ashape[1], \
-                                                 k*ashape[2]:(k+1)*ashape[2]]=\
-                                                data-self.__Min[key]
-            self.Ea[key] = self.GetEa(self.ndata)
-
-        #print('BVSE Ea is {0},\nBVEL Ea is {1}'.format(self.BVSEEa,self.BVELEa))
-        return True
-
-    def GetEa(self, data):
-        return [self.GetConnectEa(data,1),\
-                self.GetConnectEa(data,2),\
-                self.GetConnectEa(data,3)]
-
-    def GetConnectEa(self, data, connectnumber):
-        minvalue = 0.0
-        maxvalue = 20.0
-        while (maxvalue - minvalue) > 0.01:
-            testvalue = (maxvalue + minvalue) / 2.0
-            testdata = data < testvalue
-            number = self.CaluRegionConnectivity(testdata)
-            if number >= connectnumber:
-                maxvalue = testvalue
-            else:
-                minvalue = testvalue
-        if maxvalue >= 20.0:
-            return 20000
-        else:
-            return maxvalue
-
-    def CaluRegionConnectivity(self, region):
-        struct = scipy.ndimage.generate_binary_structure(3, 3)
-        lw, num = measurements.label(region, structure=struct)
-        sliced = measurements.find_objects(lw)
-        connectnumber = np.zeros(num, dtype=np.int)
-        if (num > 0):
-            for index, slic in enumerate(sliced):
-                for i in range(len(slic)):
-                    if ((slic[i].start == 0)
-                            and slic[i].stop == region.shape[i]):
-                        connectnumber[index] = connectnumber[index] + 1
-        return np.max(connectnumber)
-
-    # def write_vti_file(self,filename='test.vti'):
-    # imageData = vtk.vtkImageData()
-    # imageData.SetDimensions(self._Size)
-    # self._reslen=0.1
-    # imageData.SetSpacing(self._reslen,self._reslen,self._reslen)
-    # imageData.AllocateScalars(vtk.VTK_FLOAT, 1)
-    # for k in range(self._Size[2]):
-    # for j in range(self._Size[1]):
-    # for i in range(self._Size[0]):
-    # imageData.SetScalarComponentFromDouble(i, j,k, 0, self.__Data['BVSE'][i][j][k])
-    # writer = vtk.vtkXMLImageDataWriter()
-    # writer.SetFileName(filename)
-    # writer.SetInputData(imageData)
-    # writer.Write()
-
-    Data = property(get_data, set_data, del_data, "Data's docstring")
-    Max = property(get_max, set_max, del_max, "Max's docstring")
-    Min = property(get_min, set_min, del_min, "Min's docstring")
-
-
-# if __name__=="__main__":
-#     bvmdata=loadbvparam('bvmparam.data')
-#
-#     print(bvmdata['Na'+'1'+'O'+'-2'])
+'''
+Created on 2017
+
+@author: hebing
+'''
+import os
+import numpy as np
+from scipy.special import erfc
+from scipy.ndimage import measurements
+import scipy.ndimage
+import math
+from struct import pack
+
+
+def loadbvparam(filename):
+    with open(filename, 'r') as fp:
+        lines = fp.readlines()
+    bvmpara = {}
+    for line in lines:
+        varstr = line.split('\t')
+        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
+        if key in bvmpara:
+            bvmpara[key].append([float(varstr[4]), float(varstr[5])])
+        else:
+            bvmpara[key] = [[float(varstr[4]), float(varstr[5])]]
+    return bvmpara
+
+
+def loadBVSEparam(filename):
+    with open(filename, 'r') as fp:
+        lines = fp.readlines()
+    BVSEparam = {}
+    for line in lines[1:]:
+        line = line.strip('\n')
+        varstr = line.split('\t')
+        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
+        if key in BVSEparam:
+            BVSEparam[key].append([
+                float(varstr[4]),
+                float(varstr[5]),
+                float(varstr[6]),
+                float(varstr[7]),
+                float(varstr[8]),
+                float(varstr[9])
+            ])
+        else:
+            BVSEparam[key] = [[
+                float(varstr[4]),
+                float(varstr[5]),
+                float(varstr[6]),
+                float(varstr[7]),
+                float(varstr[8]),
+                float(varstr[9])
+            ]]
+    return BVSEparam
+
+
+def loadElementsparam(filename):
+    with open(filename, 'r') as fp:
+        lines = fp.readlines()
+    Elementsparam = {}
+    for line in lines:
+        line = line.strip('\n')
+        varstr = line.split('\t')
+        key = varstr[1] + varstr[2]
+        Elementsparam[key] = [
+            float(varstr[0]),
+            float(varstr[3]),
+            float(varstr[4]),
+            float(varstr[5]),
+            float(varstr[6]),
+            float(varstr[7]),
+            float(varstr[8]),
+            float(varstr[9])
+        ]
+    return Elementsparam
+
+
+class BVAnalysis(object):
+    '''
+    for bond valence method analyze ion channel
+    '''
+
+    def __init__(self, struc=None, size=[50, 50, 50]):
+        '''
+        Constructor
+        '''
+        self._Struct = struc
+        self._Size = [50, 50, 50]
+        self.__Data = {}
+        self.__Max = {}
+        self.__Min = {}
+        self.Ea = {}
+        self._MoveIon = 'Li'
+        self._poss = None
+        self.ValenceOfMoveIon = 1
+        self.stop = False
+        module_dir = os.path.dirname(os.path.abspath(__file__))
+
+        self._BVparam = loadbvparam(os.path.join(module_dir, 'bvmparam.dat'))
+        self._BVSEparam = loadBVSEparam(os.path.join(module_dir, 'bvse.dat'))
+        self._Elementsparam = loadElementsparam(
+            os.path.join(module_dir, 'elements.dat'))
+
+    def get_data(self):
+        return self.__Data
+
+    def get_max(self):
+        return self.__Max
+
+    def get_min(self):
+        return self.__Min
+
+    def set_data(self, value):
+        self.__Data = value
+
+    def set_max(self, value):
+        self.__Max = value
+
+    def set_min(self, value):
+        self.__Min = value
+
+    def del_data(self):
+        del self.__Data
+
+    def del_max(self):
+        del self.__Max
+
+    def del_min(self):
+        del self.__Min
+
+    @property
+    def BVSMin(self):
+        return self.__Min['BVS']
+
+    @property
+    def BVSEMin(self):
+        return self.__Min['BVSE']
+
+    @property
+    def BVELMin(self):
+        return self.__Min['BVEL']
+
+    @property
+    def BVSMax(self):
+        return self.__Max['BVS']
+
+    @property
+    def BVSEMax(self):
+        return self.__Max['BVSE']
+
+    @property
+    def BVELMax(self):
+        return self.__Max['BVEL']
+
+    @property
+    def BVSEEa(self):
+        return self.Ea['BVSE']
+
+    @property
+    def BVELEa(self):
+        return self.Ea['BVEL']
+
+    def SetStructure(self, struc):
+        self._Struct = struc
+
+    def SetMoveIon(self, moveion):
+        self._MoveIon = moveion
+
+    def SetResolution(self, size):
+        self._Size = size
+
+    def SetLengthResolution(self, reslen=0.1):
+        abc = self._Struct.Getabc()
+        self._reslen = reslen
+        self._Size[0] = int(abc[0] / reslen) + 1
+        self._Size[1] = int(abc[1] / reslen) + 1
+        self._Size[2] = int(abc[2] / reslen) + 1
+
+    def SaveBVSEData(self, filename):
+        self.SaveBinaryData(filename + '_BVSE.pgrid', self.__Data['BVSE'],
+                            'BVSE')
+        np.save(filename + "_BVSE.npy", self.__Data['BVSE'])
+
+    def SaveBVELData(self, filename):
+        self.SaveBinaryData(filename + '_BVEL.pgrid', self.__Data['BVEL'],
+                            'BVEL')
+
+    def SaveBVSData(self, filename):
+        self.SaveBinaryData(filename + '_BVS.pgrid', self.__Data['BVS'], 'BVS')
+
+    def SaveData(self, filename, data, datatype=' '):
+        fp = open(filename, 'w')
+        fp.write(datatype + '\n')
+        alpha = self._Struct.GetAlphaBetaGama()
+        abc = self._Struct.Getabc()
+        fp.write(str(abc[0]) + ' ' + str(abc[1]) + ' ' + str(abc[2]) + ' ')
+        fp.write(
+            str(alpha[0]) + ' ' + str(alpha[1]) + ' ' + str(alpha[2]) + '\n')
+        fp.write(
+            str(self._Size[0]) + ' ' + str(self._Size[1]) + ' ' +
+            str(self._Size[2]) + '\n ')
+        for i in range(self._Size[0]):
+            for j in range(self._Size[1]):
+                for k in range(self._Size[2]):
+                    fp.write(str(data[i][j][k]) + '\n')
+        fp.close()
+
+    def SaveBinaryData(self, filename, data, datatype=' '):
+        latticeparam = self._Struct.Getabc() + self._Struct.GetAlphaBetaGama()
+        with open(filename, 'wb') as outf:
+            outf.write(pack('4i', 3, 0, 0, 0))  # file format version
+            outf.write(pack(
+                '80s',
+                datatype.ljust(80).encode('utf-8')))  # Title 80 characters
+            outf.write(pack('i', 1))  # gType 0 for *.ggrid, 1 for *.pgrid
+            outf.write(pack('i', 0))  # fType 0
+            outf.write(pack('i', 1))  # nVal dummy
+            outf.write(pack('i', 3))  # dimension
+            outf.write(pack('3i', *self._Size))  # numbers of voxels
+            outf.write(pack('i', data.size))  # Total number of voxels
+            outf.write(pack('6f', *latticeparam))  # lattice parameters
+            for k in range(self._Size[2]):
+                for j in range(self._Size[1]):
+                    for i in range(self._Size[0]):
+                        outf.write(pack('f', data[i][j][k]))
+
+    def ReadData(self, filename, data, datatype=' '):
+        fp = open(filename, 'r')
+        datatype = fp.readline()
+        alpha = self._Struct.GetAlphaBetaGama()
+        abc = self._Struct.Getabc()
+        abc = fp.readline().split()
+        alpha = fp.readline().split()
+        strs = fp.readline().split()
+        size = [int(i) for i in strs]
+        if datatype == 'bvs':
+            self.__Data['BVS'] = np.zeros(size)
+            data = self.__Data['BVS']
+        else:
+            self.__Data['BVSE'] = np.zeros(size)
+            data = self.__Data['BVSE']
+        for i in range(size[2]):
+            for j in range(size[1]):
+                for k in range(size[0]):
+                    strs = fp.readline().split()
+                    data[k][j][i] = int(strs[0])
+
+        fp.close()
+
+    def GetBVSData(self):
+        return self.__Data['BVS']
+
+    def GetBVSEData(self):
+        return self.__Data['BVSE']
+
+    def GetPosSet(self):
+        return self._poss
+
+    def CaluGlobalIndex(self, ):
+        self.stop = False
+        self._Size.reverse()
+        centrepos = np.zeros(self._Size + [3])
+        self._Data = np.zeros(self._Size, dtype=np.double)
+        for k in range(self._Size[0]):
+            for j in range(self._Size[1]):
+                for i in range(self._Size[2]):
+                    centrepos[k][j][i][2] = k / (self._Size[0] - 1.0)
+                    centrepos[k][j][i][1] = j / (self._Size[1] - 1.0)
+                    centrepos[k][j][i][0] = i / (self._Size[2] - 1.0)
+
+        self._poss = self._Struct.FracPosToCartPos(centrepos)
+        (distance, neighborsindex) = self._Struct.GetKNeighbors(self._poss,
+                                                                kn=8)
+
+        site2atoms = None
+        for k in range(self._Size[0]):
+
+            for j in range(self._Size[1]):
+                for i in range(self._Size[2]):
+                    if self.stop:
+                        return
+                    for dindex, index in enumerate(neighborsindex[k][j][i]):
+                        site2 = self._Struct.GetSuperCellusites()[index]
+                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
+                            for key in site2.GetElementsOccupy():
+                                if key != 'Vac':
+                                    site2atoms = key
+                            if self.ValenceOfMoveIon > 0:
+                                key = "".join([
+                                    self._MoveIon,
+                                    str(self.ValenceOfMoveIon), site2atoms,
+                                    str(site2.GetElementsOxiValue()
+                                        [site2atoms])
+                                ])
+                            else:
+                                key = "".join([
+                                    site2atoms,
+                                    str(site2.GetElementsOxiValue()
+                                        [site2atoms]), self._MoveIon,
+                                    str(self.ValenceOfMoveIon)
+                                ])
+                            if key in self._BVparam:
+                                (r, b) = self._BVparam[key][0]
+                                bv = np.exp(
+                                    (r - distance[k][j][i][dindex]) / b)
+                                self.__Data['BVS'][k][j][
+                                    i] = self.__Data['BVS'][k][j][i] + bv
+                            else:
+                                print('Not Find bvs param' + key)
+                        else:
+                            pass
+                            #print(site2.GetSiteLabel())
+    def CaluBVSE(self, ProgressCall):
+        if len(self._Struct._OxidationTable) == 0:
+            raise Exception(
+                "can't caculation bvs and Ea without atom oxi info !")
+        self.stop = False
+        centrepos = np.zeros(self._Size + [3])
+        self.__Data['BVS'] = np.zeros(self._Size, dtype=np.double)
+        self.__Data['BVSE'] = np.zeros(self._Size, dtype=np.double)
+        self.__Data['BVEL'] = np.zeros(self._Size, dtype=np.double)
+        for k in range(self._Size[2]):
+            for j in range(self._Size[1]):
+                for i in range(self._Size[0]):
+                    centrepos[i][j][k][2] = k / (self._Size[2] - 1.0)
+                    centrepos[i][j][k][1] = j / (self._Size[1] - 1.0)
+                    centrepos[i][j][k][0] = i / (self._Size[0] - 1.0)
+        if ProgressCall:
+            ProgressCall(10)
+        self._poss = self._Struct.FracPosToCartPos(centrepos)
+
+        atomsq = {}
+        for atom in self._Struct._atomsymbols:
+            atomsq[atom] = 0
+            for site in self._Struct._Sites:
+                if atom in site.GetElements():
+                    key = atom + str(site.GetElementsOxiValue()[atom])
+                    atomsq[atom] = atomsq[atom] + site.GetElementsOxiValue(
+                    )[atom] * site.GetElementsOccupy()[atom] / math.sqrt(
+                        self._Elementsparam[key][3])
+        qsumanion = 0
+        qsumcation = 0
+        for (atom, value) in atomsq.items():
+            if value > 0:
+                qsumcation = qsumcation + value
+            elif value < 0:
+                qsumanion = qsumanion + value
+            else:
+                qsumanion = 0
+                qsumcation = 0
+        qsum = 0.0
+        if self.ValenceOfMoveIon > 0:
+            qsum = -qsumanion / qsumcation
+        else:
+            qsum = -qsumcation / qsumanion
+        key1 = self._MoveIon + str(self.ValenceOfMoveIon)
+        qm1 = self.ValenceOfMoveIon / math.sqrt(self._Elementsparam[key1][3])
+        rm1 = self._Elementsparam[key1][6]
+        for i in range(self._Size[0]):
+            (distance,
+             neighborsindex) = self._Struct.GetKNeighbors(self._poss[i],
+                                                          kn=128)
+            if ProgressCall:
+                ProgressCall(10 + i * 90 / (self._Size[0] - 1))
+            for j in range(self._Size[1]):
+                for k in range(self._Size[2]):
+                    if self.stop:
+                        return False
+                    bvsdata = 0.0
+                    data = 0.0
+                    cdata = 0.0
+                    bvelcdata = 0.0
+                    N = 0
+                    D0 = 0.0
+                    Rcutoff = 10.0
+                    alpha = 0.0
+                    occupyvalue = 0.0
+                    for dindex, index in enumerate(neighborsindex[j][k]):
+                        site2 = self._Struct._SuperCellusites[index]
+                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
+                            for (ssymbol, occupyvalue
+                                 ) in site2.GetElementsOccupy().items():
+                                if ssymbol != 'Vac':
+                                    site2oxi = site2.GetElementsOxiValue(
+                                    )[ssymbol]
+                                    if self.ValenceOfMoveIon > 0:
+                                        key = "".join([
+                                            self._MoveIon,
+                                            str(self.ValenceOfMoveIon),
+                                            ssymbol,
+                                            str(site2oxi)
+                                        ])
+                                    else:
+                                        key = "".join([
+                                            ssymbol,
+                                            str(site2oxi), self._MoveIon,
+                                            str(self.ValenceOfMoveIon)
+                                        ])
+                                    if (key in self._BVSEparam) and (
+                                            key in self._BVparam):
+                                        (Nc, r0, Rcutoff, D0, Rmin,
+                                         alpha) = self._BVSEparam[key][0]
+                                        (r, b) = self._BVparam[key][0]
+                                        Rcutoff = 10.0
+                                        if distance[j][k][dindex] <= Rcutoff:
+                                            # bv=np.exp((r0-distance[k][j][i][dindex])*alpha)
+                                            bvs = np.exp(
+                                                (r - distance[j][k][dindex]) /
+                                                b)
+                                            smin = np.exp(
+                                                (Rmin - distance[j][k][dindex])
+                                                * alpha)
+                                            en_s = np.exp(
+                                                (Rmin - Rcutoff) * alpha)
+                                            bvsdata = bvsdata + bvs  #*occupyvalue-((en_s-1)**2-1)
+                                            data = data + ((smin - 1)**2 -
+                                                           1) * occupyvalue
+                                    else:
+                                        if (key not in self._BVSEparam):
+                                            raise Exception(
+                                                "bvse {0}  param can't find!!!!"
+                                                .format(key))
+                                            ProgressCall(0)
+                                        else:
+                                            raise Exception(
+                                                "bvs {0} param can't find!!!!".
+                                                format(key))
+                                            ProgressCall(0)
+                        else:
+                            for (ssymbol, occupyvalue
+                                 ) in site2.GetElementsOccupy().items():
+                                if ssymbol != 'Vac':
+                                    site2oxi = site2.GetElementsOxiValue(
+                                    )[ssymbol]
+                                    if ssymbol != self._MoveIon:
+                                        key = ssymbol + str(site2oxi)
+                                        rm2 = self._Elementsparam[key][6]
+                                        qm2 = site2oxi / math.sqrt(
+                                            self._Elementsparam[key][3])
+                                        rm1m2 = distance[j][k][dindex]
+                                        f = 0.74
+                                        if rm1m2 > rm2:
+                                            if rm1m2 < Rcutoff:
+                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(
+                                                    rm1m2 /
+                                                    (f * (rm1 + rm2))) * qsum
+                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (
+                                                    erfc(rm1m2 /
+                                                         (f * (rm1 + rm2))) -
+                                                    erfc(Rcutoff /
+                                                         (f * (rm1 + rm2))))
+                                        else:
+                                            cdata = 300
+                                            bvelcdata = 300
+                    self.__Data['BVSE'][i][j][k] = (0.5 * D0 * (data) +
+                                                    14.4 * cdata)
+                    self.__Data['BVS'][i][j][k] = bvsdata
+                    self.__Data['BVEL'][i][j][k] = (D0 * (data) +
+                                                    14.4 * bvelcdata)
+        self.__Data['BVSE'] = self.__Data['BVSE']  #/self.ValenceOfMoveIon
+        self.__Data['BVEL'] = self.__Data['BVEL']  #/self.ValenceOfMoveIon
+        for key, data in self.__Data.items():
+            self.__Max[key] = np.max(data)
+            self.__Min[key] = np.min(data)
+            ashape = self.__Data['BVSE'].shape
+            self.ndata = np.zeros(
+                (2 * ashape[0], 2 * ashape[1], 2 * ashape[2]))
+            for i in range(2):
+                for j in range(2):
+                    for k in range(2):
+                        self.ndata[i*ashape[0]:(i+1)*ashape[0], \
+                                                 j*ashape[1]:(j+1)*ashape[1], \
+                                                 k*ashape[2]:(k+1)*ashape[2]]=\
+                                                data-self.__Min[key]
+            self.Ea[key] = self.GetEa(self.ndata)
+
+        #print('BVSE Ea is {0},\nBVEL Ea is {1}'.format(self.BVSEEa,self.BVELEa))
+        return True
+
+    def GetEa(self, data):
+        return [self.GetConnectEa(data,1),\
+                self.GetConnectEa(data,2),\
+                self.GetConnectEa(data,3)]
+
+    def GetConnectEa(self, data, connectnumber):
+        minvalue = 0.0
+        maxvalue = 20.0
+        while (maxvalue - minvalue) > 0.01:
+            testvalue = (maxvalue + minvalue) / 2.0
+            testdata = data < testvalue
+            number = self.CaluRegionConnectivity(testdata)
+            if number >= connectnumber:
+                maxvalue = testvalue
+            else:
+                minvalue = testvalue
+        if maxvalue >= 20.0:
+            return 20000
+        else:
+            return maxvalue
+
+    def CaluRegionConnectivity(self, region):
+        struct = scipy.ndimage.generate_binary_structure(3, 3)
+        lw, num = measurements.label(region, structure=struct)
+        sliced = measurements.find_objects(lw)
+        connectnumber = np.zeros(num, dtype=np.int)
+        if (num > 0):
+            for index, slic in enumerate(sliced):
+                for i in range(len(slic)):
+                    if ((slic[i].start == 0)
+                            and slic[i].stop == region.shape[i]):
+                        connectnumber[index] = connectnumber[index] + 1
+        return np.max(connectnumber)
+
+    # def write_vti_file(self,filename='test.vti'):
+    # imageData = vtk.vtkImageData()
+    # imageData.SetDimensions(self._Size)
+    # self._reslen=0.1
+    # imageData.SetSpacing(self._reslen,self._reslen,self._reslen)
+    # imageData.AllocateScalars(vtk.VTK_FLOAT, 1)
+    # for k in range(self._Size[2]):
+    # for j in range(self._Size[1]):
+    # for i in range(self._Size[0]):
+    # imageData.SetScalarComponentFromDouble(i, j,k, 0, self.__Data['BVSE'][i][j][k])
+    # writer = vtk.vtkXMLImageDataWriter()
+    # writer.SetFileName(filename)
+    # writer.SetInputData(imageData)
+    # writer.Write()
+
+    Data = property(get_data, set_data, del_data, "Data's docstring")
+    Max = property(get_max, set_max, del_max, "Max's docstring")
+    Min = property(get_min, set_min, del_min, "Min's docstring")
+
+
+# if __name__=="__main__":
+#     bvmdata=loadbvparam('bvmparam.data')
+#
+#     print(bvmdata['Na'+'1'+'O'+'-2'])
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,571 +1,571 @@
-# -*- coding: utf-8 -*-
-'''
-Origin code info:
-    Created on 2017
-    author: hebing
-
-Modify info:
-    modify author: Bowei Pu
-    version: 2022.08.17
-    function:
-        Consider mobile ion when cal bv
-'''
-import os
-import numpy as np
-from scipy.special import erfc
-from scipy.ndimage import measurements
-import scipy.ndimage
-import math
-from struct import pack
-from tqdm import tqdm
-
-
-def loadbvparam(filename):
-    with open(filename, 'r') as fp:
-        lines = fp.readlines()
-    bvmpara = {}
-    for line in lines:
-        varstr = line.split('\t')
-        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
-        if key in bvmpara:
-            bvmpara[key].append([float(varstr[4]), float(varstr[5])])
-        else:
-            bvmpara[key] = [[float(varstr[4]), float(varstr[5])]]
-    return bvmpara
-
-
-def loadBVSEparam(filename):
-    with open(filename, 'r') as fp:
-        lines = fp.readlines()
-    BVSEparam = {}
-    for line in lines[1:]:
-        line = line.strip('\n')
-        varstr = line.split('\t')
-        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
-        if key in BVSEparam:
-            BVSEparam[key].append([
-                float(varstr[4]),
-                float(varstr[5]),
-                float(varstr[6]),
-                float(varstr[7]),
-                float(varstr[8]),
-                float(varstr[9])
-            ])
-        else:
-            BVSEparam[key] = [[
-                float(varstr[4]),
-                float(varstr[5]),
-                float(varstr[6]),
-                float(varstr[7]),
-                float(varstr[8]),
-                float(varstr[9])
-            ]]
-    return BVSEparam
-
-
-def loadElementsparam(filename):
-    with open(filename, 'r') as fp:
-        lines = fp.readlines()
-    Elementsparam = {}
-    for line in lines:
-        line = line.strip('\n')
-        varstr = line.split('\t')
-        key = varstr[1] + varstr[2]
-        Elementsparam[key] = [
-            float(varstr[0]),
-            float(varstr[3]),
-            float(varstr[4]),
-            float(varstr[5]),
-            float(varstr[6]),
-            float(varstr[7]),
-            float(varstr[8]),
-            float(varstr[9])
-        ]
-    return Elementsparam
-
-
-class BVAnalysis(object):
-    '''
-    for bond valence method analyze ion channel
-    '''
-
-    def __init__(self, struc=None, size=[50, 50, 50]):
-        '''
-        Constructor
-        '''
-        self._Struct = struc
-        self._Size = [50, 50, 50]
-        self.__Data = {}
-        self.__Max = {}
-        self.__Min = {}
-        self.Ea = {}
-        self._MoveIon = 'Li'
-        self._poss = None
-        self.ValenceOfMoveIon = 1
-        self.stop = False
-        module_dir = os.path.dirname(os.path.abspath(__file__))
-
-        self._BVparam = loadbvparam(os.path.join(module_dir, 'bvmparam.dat'))
-        self._BVSEparam = loadBVSEparam(os.path.join(module_dir, 'bvse.dat'))
-        self._Elementsparam = loadElementsparam(os.path.join(module_dir, 'elements.dat'))
-
-    def get_data(self):
-        return self.__Data
-
-    def get_max(self):
-        return self.__Max
-
-    def get_min(self):
-        return self.__Min
-
-    def set_data(self, value):
-        self.__Data = value
-
-    def set_max(self, value):
-        self.__Max = value
-
-    def set_min(self, value):
-        self.__Min = value
-
-    def del_data(self):
-        del self.__Data
-
-    def del_max(self):
-        del self.__Max
-
-    def del_min(self):
-        del self.__Min
-
-    @property
-    def BVSMin(self):
-        return self.__Min['BVS']
-
-    @property
-    def BVSEMin(self):
-        return self.__Min['BVSE']
-
-    @property
-    def BVELMin(self):
-        return self.__Min['BVEL']
-
-    @property
-    def BVSMax(self):
-        return self.__Max['BVS']
-
-    @property
-    def BVSEMax(self):
-        return self.__Max['BVSE']
-
-    @property
-    def BVELMax(self):
-        return self.__Max['BVEL']
-
-    @property
-    def BVSEEa(self):
-        return self.Ea['BVSE']
-
-    @property
-    def BVELEa(self):
-        return self.Ea['BVEL']
-
-    def SetStructure(self, struc):
-        self._Struct = struc
-
-    def SetMoveIon(self, moveion):
-        self._MoveIon = moveion
-
-    def SetResolution(self, size):
-        self._Size = size
-
-    def SetLengthResolution(self, reslen=0.1):
-        abc = self._Struct.Getabc()
-        self._reslen = reslen
-        self._Size[0] = int(abc[0] / reslen) + 1
-        self._Size[1] = int(abc[1] / reslen) + 1
-        self._Size[2] = int(abc[2] / reslen) + 1
-
-    def SaveBVSEData(self, filename):
-        self.SaveBinaryData('{}_BVSELi.pgrid'.format(filename), self.__Data['BVSE'], 'BVSE')
-        np.save('{}_BVSELi.npy'.format(filename), self.__Data['BVSE'])
-
-    def SaveBVELData(self, filename):
-        self.SaveBinaryData('{}_BVELLi.pgrid'.format(filename), self.__Data['BVEL'], 'BVEL')
-        # np.save('{}_BVELLi.npy'.format(filename), self.__Data['BVEL'])
-
-    def SaveBVSData(self, filename):
-        self.SaveBinaryData('{}_BVSLi.pgrid'.format(filename), self.__Data['BVS'], 'BVS')
-        # np.save('{}_BVSLi.npy'.format(filename), self.__Data['BVS'])
-
-    def SaveData(self, filename, data, datatype=' '):
-        fp = open(filename, 'w')
-        fp.write(datatype + '\n')
-        alpha = self._Struct.GetAlphaBetaGama()
-        abc = self._Struct.Getabc()
-        fp.write(str(abc[0]) + ' ' + str(abc[1]) + ' ' + str(abc[2]) + ' ')
-        fp.write(str(alpha[0]) + ' ' + str(alpha[1]) + ' ' + str(alpha[2]) + '\n')
-        fp.write(str(self._Size[0]) + ' ' + str(self._Size[1]) + ' ' + str(self._Size[2]) + '\n ')
-        for i in range(self._Size[0]):
-            for j in range(self._Size[1]):
-                for k in range(self._Size[2]):
-                    fp.write(str(data[i][j][k]) + '\n')
-        fp.close()
-
-    def SaveBinaryData(self, filename, data, datatype=' '):
-        latticeparam = self._Struct.Getabc() + self._Struct.GetAlphaBetaGama()
-        with open(filename, 'wb') as outf:
-            outf.write(pack('4i', 3, 0, 0, 0))  # file format version
-            outf.write(pack(
-                '80s',
-                datatype.ljust(80).encode('utf-8')))  # Title 80 characters
-            outf.write(pack('i', 1))  # gType 0 for *.ggrid, 1 for *.pgrid
-            outf.write(pack('i', 0))  # fType 0
-            outf.write(pack('i', 1))  # nVal dummy
-            outf.write(pack('i', 3))  # dimension
-            outf.write(pack('3i', *self._Size))  # numbers of voxels
-            outf.write(pack('i', data.size))  # Total number of voxels
-            outf.write(pack('6f', *latticeparam))  # lattice parameters
-            for k in range(self._Size[2]):
-                for j in range(self._Size[1]):
-                    for i in range(self._Size[0]):
-                        outf.write(pack('f', data[i][j][k]))
-
-    def ReadData(self, filename, data, datatype=' '):
-        fp = open(filename, 'r')
-        datatype = fp.readline()
-        alpha = self._Struct.GetAlphaBetaGama()
-        abc = self._Struct.Getabc()
-        abc = fp.readline().split()
-        alpha = fp.readline().split()
-        strs = fp.readline().split()
-        size = [int(i) for i in strs]
-        if datatype == 'bvs':
-            self.__Data['BVS'] = np.zeros(size)
-            data = self.__Data['BVS']
-        else:
-            self.__Data['BVSE'] = np.zeros(size)
-            data = self.__Data['BVSE']
-        for i in range(size[2]):
-            for j in range(size[1]):
-                for k in range(size[0]):
-                    strs = fp.readline().split()
-                    data[k][j][i] = int(strs[0])
-        fp.close()
-
-    def GetBVSData(self):
-        return self.__Data['BVS']
-
-    def GetBVSEData(self):
-        return self.__Data['BVSE']
-
-    def GetPosSet(self):
-        return self._poss
-
-    def CaluGlobalIndex(self):
-        self.stop = False
-        self._Size.reverse()
-        centrepos = np.zeros(self._Size + [3])
-        self._Data = np.zeros(self._Size, dtype=np.double)
-        for k in range(self._Size[0]):
-            for j in range(self._Size[1]):
-                for i in range(self._Size[2]):
-                    centrepos[k][j][i][2] = k / (self._Size[0] - 1.0)
-                    centrepos[k][j][i][1] = j / (self._Size[1] - 1.0)
-                    centrepos[k][j][i][0] = i / (self._Size[2] - 1.0)
-
-        self._poss = self._Struct.FracPosToCartPos(centrepos)
-        (distance, neighborsindex) = self._Struct.GetKNeighbors(self._poss, kn=8)
-
-        site2atoms = None
-        for k in range(self._Size[0]):
-            for j in range(self._Size[1]):
-                for i in range(self._Size[2]):
-                    if self.stop:
-                        return
-                    
-                    for dindex, index in enumerate(neighborsindex[k][j][i]):
-                        site2 = self._Struct.GetSuperCellusites()[index]
-                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
-                            for key in site2.GetElementsOccupy():
-                                if key != 'Vac':
-                                    site2atoms = key
-                            if self.ValenceOfMoveIon > 0:
-                                key = "".join([self._MoveIon, str(self.ValenceOfMoveIon), site2atoms, str(site2.GetElementsOxiValue()[site2atoms])])
-                            else:
-                                key = "".join([site2atoms, str(site2.GetElementsOxiValue()[site2atoms]), self._MoveIon, str(self.ValenceOfMoveIon)])
-                            if key in self._BVparam:
-                                (r, b) = self._BVparam[key][0]
-                                bv = np.exp((r - distance[k][j][i][dindex]) / b)
-                                self.__Data['BVS'][k][j][i] = self.__Data['BVS'][k][j][i] + bv
-                            else:
-                                print('Not Find bvs param' + key)
-                        else:
-                            pass
-                            # print(site2.GetSiteLabel())
-    
-    def CaluBVSE(self, ProgressCall, Rmin_moveion=3):
-        self.Rmin_moveion = Rmin_moveion
-        
-        if len(self._Struct._OxidationTable) == 0:
-            raise Exception('can not calculate BV and Ea without atom oxi info')
-        
-        self.stop = False
-        
-        centrepos = np.zeros(self._Size + [3])
-        self.__Data['BVS'] = np.zeros(self._Size, dtype=np.double)
-        self.__Data['BVSE'] = np.zeros(self._Size, dtype=np.double)
-        self.__Data['BVEL'] = np.zeros(self._Size, dtype=np.double)
-        
-        for k in range(self._Size[2]):
-            for j in range(self._Size[1]):
-                for i in range(self._Size[0]):
-                    centrepos[i][j][k][2] = k / (self._Size[2] - 1.0)
-                    centrepos[i][j][k][1] = j / (self._Size[1] - 1.0)
-                    centrepos[i][j][k][0] = i / (self._Size[0] - 1.0)
-        
-        if ProgressCall:
-            ProgressCall(0)
-        
-        self._poss = self._Struct.FracPosToCartPos(centrepos)
-
-        atomsq = {}
-        for atom in self._Struct._atomsymbols:
-            atomsq[atom] = 0
-            for site in self._Struct._Sites:
-                if atom in site.GetElements():
-                    key = atom + str(site.GetElementsOxiValue()[atom])
-                    atomsq[atom] = atomsq[atom] + site.GetElementsOxiValue()[atom] * site.GetElementsOccupy()[atom] / math.sqrt(self._Elementsparam[key][3])
-        
-        qsumanion = 0
-        qsumcation = 0
-        for (atom, value) in atomsq.items():
-            if value > 0:
-                qsumcation = qsumcation + value
-            elif value < 0:
-                qsumanion = qsumanion + value
-            else:
-                qsumanion = 0
-                qsumcation = 0
-        
-        qsum = 0.0
-        if self.ValenceOfMoveIon > 0:
-            qsum = -qsumanion / qsumcation
-        else:
-            qsum = -qsumcation / qsumanion
-        
-        key1 = self._MoveIon + str(self.ValenceOfMoveIon)
-        qm1 = self.ValenceOfMoveIon / math.sqrt(self._Elementsparam[key1][3])
-        rm1 = self._Elementsparam[key1][6]
-        
-        ## tqdm color: '#00ff00', 'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white'
-        for i in tqdm(range(self._Size[0]), colour='cyan', desc=None):
-            (distance, neighborsindex) = self._Struct.GetKNeighbors(self._poss[i], kn=128)
-            
-            if ProgressCall:
-                ProgressCall(10 + i * 90 / (self._Size[0] - 1))
-            
-            for j in tqdm(range(self._Size[1]), colour=None, leave=False):
-                
-                ## Single calculation is too fast, not need to use k loop tqdm
-                # for k in tqdm(range(self._Size[2]), colour='black', leave=False):
-                for k in range(self._Size[2]):
-                    
-                    if self.stop:
-                        return False
-                    
-                    bvsdata = 0.0
-                    data = 0.0
-                    cdata = 0.0
-                    bvelcdata = 0.0
-                    N = 0
-                    D0 = 0.0
-                    Rcutoff = 10.0
-                    alpha = 0.0
-                    occupyvalue = 0.0
-                    
-                    list_cdata_Li = []
-                    list_bvelcdata_Li = []
-                    
-                    break_this_point = False
-                    exclude_NN_Li = False
-                    
-                    for dindex, index in enumerate(neighborsindex[j][k]):
-                        if break_this_point:
-                            break
-                        
-                        ## site2 is the neighbor of attempt_Li+
-                        site2 = self._Struct._SuperCellusites[index]
-                        
-                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
-                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
-                                if ssymbol != 'Vac':
-                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
-                                    if self.ValenceOfMoveIon > 0:
-                                        key = "".join([self._MoveIon, str(self.ValenceOfMoveIon), ssymbol, str(site2oxi)])
-                                    else:
-                                        key = "".join([ssymbol, str(site2oxi), self._MoveIon, str(self.ValenceOfMoveIon)])
-                                    if (key in self._BVSEparam) and (key in self._BVparam):
-                                        (Nc, r0, Rcutoff, D0, Rmin, alpha) = self._BVSEparam[key][0]
-                                        (r, b) = self._BVparam[key][0]
-                                        Rcutoff = 10.0
-                                        if distance[j][k][dindex] <= Rcutoff:
-                                            # bv=np.exp((r0-distance[k][j][i][dindex])*alpha)
-                                            bvs = np.exp((r - distance[j][k][dindex]) / b)
-                                            smin = np.exp((Rmin - distance[j][k][dindex]) * alpha)
-                                            en_s = np.exp((Rmin - Rcutoff) * alpha)
-                                            bvsdata = bvsdata + bvs  #*occupyvalue-((en_s-1)**2-1)
-                                            data = data + ((smin - 1)**2 - 1) * occupyvalue
-                                    else:
-                                        if (key not in self._BVSEparam):
-                                            raise Exception("bvse {0}  param can't find!!!!".format(key))
-                                            ProgressCall(0)
-                                        else:
-                                            raise Exception("bvs {0} param can't find!!!!".format(key))
-                                            ProgressCall(0)
-                        else:
-                            ## When Li+, this if-else is for effect between attempt_Li+ and *cations*
-                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
-                                if ssymbol != 'Vac':
-                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
-                                    
-                                    if ssymbol != self._MoveIon:
-                                        ## For cations around attempt_Li+, which is not Li+
-                                        key = ssymbol + str(site2oxi)
-                                        rm2 = self._Elementsparam[key][6]
-                                        qm2 = site2oxi / math.sqrt(self._Elementsparam[key][3])
-                                        rm1m2 = distance[j][k][dindex]
-                                        f = 0.74
-                                        if rm1m2 > rm2:
-                                            if rm1m2 < Rcutoff:
-                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
-                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
-                                        else:
-                                            ## For rm1m2 <= rm2, this means the sites cation is too close to attempt_Li+
-                                            ## So the calculation of this attempt_Li+ can be breaked
-                                            break_this_point = True
-                                            
-                                            cdata = 300
-                                            bvelcdata = 300
-                                    
-                                    elif ssymbol == self._MoveIon:
-                                        ## For neighbor Li+ around attempt_Li+
-                                        key = ssymbol + str(site2oxi)
-                                        rm2 = self._Elementsparam[key][6]
-                                        qm2 = site2oxi / math.sqrt(self._Elementsparam[key][3])
-                                        rm1m2 = distance[j][k][dindex]
-                                        f = 0.74
-                                        
-                                        R_strict = rm2
-                                        R_strict = self.Rmin_moveion
-                                        # R_strict = 1.45
-                                        if rm1m2 > R_strict:
-                                            if rm1m2 < Rcutoff:
-                                                # cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
-                                                # bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
-                                                
-                                                cdata_Li_i = occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
-                                                bvelcdata_Li_i = occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
-                                                
-                                                list_cdata_Li.append([rm1m2, cdata_Li_i])
-                                                list_bvelcdata_Li.append([rm1m2, bvelcdata_Li_i])
-                                                
-                                        else:
-                                            # cdata = cdata + 0
-                                            # bvelcdata = bvelcdata + 0
-                                            
-                                            pass
-                                    
-                    
-                    list_cdata_Li.sort(key=lambda x: x[0])
-                    list_cdata_Li = list_cdata_Li[1:]
-                    list_bvelcdata_Li.sort(key=lambda x: x[0])
-                    list_bvelcdata_Li = list_bvelcdata_Li[1:]
-                    
-                    cdata += sum([i[1] for i in list_cdata_Li])
-                    bvelcdata += sum([i[1] for i in list_bvelcdata_Li])
-                    
-                    self.__Data['BVSE'][i][j][k] = (0.5 * D0 * (data) + 14.4 * cdata)
-                    self.__Data['BVS'][i][j][k] = bvsdata
-                    self.__Data['BVEL'][i][j][k] = (D0 * (data) + 14.4 * bvelcdata)
-        
-        self.__Data['BVSE'] = self.__Data['BVSE']  #/self.ValenceOfMoveIon
-        self.__Data['BVEL'] = self.__Data['BVEL']  #/self.ValenceOfMoveIon
-        for key, data in self.__Data.items():
-            self.__Max[key] = np.max(data)
-            self.__Min[key] = np.min(data)
-            ashape = self.__Data['BVSE'].shape
-            self.ndata = np.zeros((2 * ashape[0], 2 * ashape[1], 2 * ashape[2]))
-            for i in range(2):
-                for j in range(2):
-                    for k in range(2):
-                        self.ndata[i*ashape[0]:(i+1)*ashape[0], \
-                                                 j*ashape[1]:(j+1)*ashape[1], \
-                                                 k*ashape[2]:(k+1)*ashape[2]]=\
-                                                data-self.__Min[key]
-            self.Ea[key] = self.GetEa(self.ndata)
-
-        _BVSE_Ea = [round(i, 2) for i in self.BVSEEa]
-        print('\nRes {} | Rmin {} | BVSE Ea {}\n'.format(self._reslen, self.Rmin_moveion, _BVSE_Ea))
-        
-        # with open('Ea.txt', 'w') as f:
-            # f.write('Res {} | Rmin {} | BVSE Ea {}\n'.format(self._reslen, self.Rmin_moveion, _BVSE_Ea))
-        
-        return True
-
-    def GetEa(self, data):
-        return [self.GetConnectEa(data,1),\
-                self.GetConnectEa(data,2),\
-                self.GetConnectEa(data,3)]
-
-    def GetConnectEa(self, data, connectnumber):
-        minvalue = 0.0
-        maxvalue = 20.0
-        while (maxvalue - minvalue) > 0.01:
-            testvalue = (maxvalue + minvalue) / 2.0
-            testdata = data < testvalue
-            number = self.CaluRegionConnectivity(testdata)
-            if number >= connectnumber:
-                maxvalue = testvalue
-            else:
-                minvalue = testvalue
-        if maxvalue >= 20.0:
-            return 20000
-        else:
-            return maxvalue
-
-    def CaluRegionConnectivity(self, region):
-        struct = scipy.ndimage.generate_binary_structure(3, 3)
-        lw, num = measurements.label(region, structure=struct)
-        sliced = measurements.find_objects(lw)
-        connectnumber = np.zeros(num, dtype=np.int)
-        if (num > 0):
-            for index, slic in enumerate(sliced):
-                for i in range(len(slic)):
-                    if ((slic[i].start == 0)
-                            and slic[i].stop == region.shape[i]):
-                        connectnumber[index] = connectnumber[index] + 1
-        return np.max(connectnumber)
-
-    # def write_vti_file(self,filename='test.vti'):
-    # imageData = vtk.vtkImageData()
-    # imageData.SetDimensions(self._Size)
-    # self._reslen=0.1
-    # imageData.SetSpacing(self._reslen,self._reslen,self._reslen)
-    # imageData.AllocateScalars(vtk.VTK_FLOAT, 1)
-    # for k in range(self._Size[2]):
-    # for j in range(self._Size[1]):
-    # for i in range(self._Size[0]):
-    # imageData.SetScalarComponentFromDouble(i, j,k, 0, self.__Data['BVSE'][i][j][k])
-    # writer = vtk.vtkXMLImageDataWriter()
-    # writer.SetFileName(filename)
-    # writer.SetInputData(imageData)
-    # writer.Write()
-
-    Data = property(get_data, set_data, del_data, "Data's docstring")
-    Max = property(get_max, set_max, del_max, "Max's docstring")
-    Min = property(get_min, set_min, del_min, "Min's docstring")
-
-
-# if __name__=="__main__":
-#     bvmdata=loadbvparam('bvmparam.data')
-#
-#     print(bvmdata['Na'+'1'+'O'+'-2'])
+# -*- coding: utf-8 -*-
+'''
+Origin code info:
+    Created on 2017
+    author: hebing
+
+Modify info:
+    modify author: Bowei Pu
+    version: 2022.08.17
+    function:
+        Consider mobile ion when cal bv
+'''
+import os
+import numpy as np
+from scipy.special import erfc
+from scipy.ndimage import measurements
+import scipy.ndimage
+import math
+from struct import pack
+from tqdm import tqdm
+
+
+def loadbvparam(filename):
+    with open(filename, 'r') as fp:
+        lines = fp.readlines()
+    bvmpara = {}
+    for line in lines:
+        varstr = line.split('\t')
+        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
+        if key in bvmpara:
+            bvmpara[key].append([float(varstr[4]), float(varstr[5])])
+        else:
+            bvmpara[key] = [[float(varstr[4]), float(varstr[5])]]
+    return bvmpara
+
+
+def loadBVSEparam(filename):
+    with open(filename, 'r') as fp:
+        lines = fp.readlines()
+    BVSEparam = {}
+    for line in lines[1:]:
+        line = line.strip('\n')
+        varstr = line.split('\t')
+        key = varstr[0] + varstr[1] + varstr[2] + varstr[3]
+        if key in BVSEparam:
+            BVSEparam[key].append([
+                float(varstr[4]),
+                float(varstr[5]),
+                float(varstr[6]),
+                float(varstr[7]),
+                float(varstr[8]),
+                float(varstr[9])
+            ])
+        else:
+            BVSEparam[key] = [[
+                float(varstr[4]),
+                float(varstr[5]),
+                float(varstr[6]),
+                float(varstr[7]),
+                float(varstr[8]),
+                float(varstr[9])
+            ]]
+    return BVSEparam
+
+
+def loadElementsparam(filename):
+    with open(filename, 'r') as fp:
+        lines = fp.readlines()
+    Elementsparam = {}
+    for line in lines:
+        line = line.strip('\n')
+        varstr = line.split('\t')
+        key = varstr[1] + varstr[2]
+        Elementsparam[key] = [
+            float(varstr[0]),
+            float(varstr[3]),
+            float(varstr[4]),
+            float(varstr[5]),
+            float(varstr[6]),
+            float(varstr[7]),
+            float(varstr[8]),
+            float(varstr[9])
+        ]
+    return Elementsparam
+
+
+class BVAnalysis(object):
+    '''
+    for bond valence method analyze ion channel
+    '''
+
+    def __init__(self, struc=None, size=[50, 50, 50]):
+        '''
+        Constructor
+        '''
+        self._Struct = struc
+        self._Size = [50, 50, 50]
+        self.__Data = {}
+        self.__Max = {}
+        self.__Min = {}
+        self.Ea = {}
+        self._MoveIon = 'Li'
+        self._poss = None
+        self.ValenceOfMoveIon = 1
+        self.stop = False
+        module_dir = os.path.dirname(os.path.abspath(__file__))
+
+        self._BVparam = loadbvparam(os.path.join(module_dir, 'bvmparam.dat'))
+        self._BVSEparam = loadBVSEparam(os.path.join(module_dir, 'bvse.dat'))
+        self._Elementsparam = loadElementsparam(os.path.join(module_dir, 'elements.dat'))
+
+    def get_data(self):
+        return self.__Data
+
+    def get_max(self):
+        return self.__Max
+
+    def get_min(self):
+        return self.__Min
+
+    def set_data(self, value):
+        self.__Data = value
+
+    def set_max(self, value):
+        self.__Max = value
+
+    def set_min(self, value):
+        self.__Min = value
+
+    def del_data(self):
+        del self.__Data
+
+    def del_max(self):
+        del self.__Max
+
+    def del_min(self):
+        del self.__Min
+
+    @property
+    def BVSMin(self):
+        return self.__Min['BVS']
+
+    @property
+    def BVSEMin(self):
+        return self.__Min['BVSE']
+
+    @property
+    def BVELMin(self):
+        return self.__Min['BVEL']
+
+    @property
+    def BVSMax(self):
+        return self.__Max['BVS']
+
+    @property
+    def BVSEMax(self):
+        return self.__Max['BVSE']
+
+    @property
+    def BVELMax(self):
+        return self.__Max['BVEL']
+
+    @property
+    def BVSEEa(self):
+        return self.Ea['BVSE']
+
+    @property
+    def BVELEa(self):
+        return self.Ea['BVEL']
+
+    def SetStructure(self, struc):
+        self._Struct = struc
+
+    def SetMoveIon(self, moveion):
+        self._MoveIon = moveion
+
+    def SetResolution(self, size):
+        self._Size = size
+
+    def SetLengthResolution(self, reslen=0.1):
+        abc = self._Struct.Getabc()
+        self._reslen = reslen
+        self._Size[0] = int(abc[0] / reslen) + 1
+        self._Size[1] = int(abc[1] / reslen) + 1
+        self._Size[2] = int(abc[2] / reslen) + 1
+
+    def SaveBVSEData(self, filename):
+        self.SaveBinaryData('{}_BVSELi.pgrid'.format(filename), self.__Data['BVSE'], 'BVSE')
+        np.save('{}_BVSELi.npy'.format(filename), self.__Data['BVSE'])
+
+    def SaveBVELData(self, filename):
+        self.SaveBinaryData('{}_BVELLi.pgrid'.format(filename), self.__Data['BVEL'], 'BVEL')
+        # np.save('{}_BVELLi.npy'.format(filename), self.__Data['BVEL'])
+
+    def SaveBVSData(self, filename):
+        self.SaveBinaryData('{}_BVSLi.pgrid'.format(filename), self.__Data['BVS'], 'BVS')
+        # np.save('{}_BVSLi.npy'.format(filename), self.__Data['BVS'])
+
+    def SaveData(self, filename, data, datatype=' '):
+        fp = open(filename, 'w')
+        fp.write(datatype + '\n')
+        alpha = self._Struct.GetAlphaBetaGama()
+        abc = self._Struct.Getabc()
+        fp.write(str(abc[0]) + ' ' + str(abc[1]) + ' ' + str(abc[2]) + ' ')
+        fp.write(str(alpha[0]) + ' ' + str(alpha[1]) + ' ' + str(alpha[2]) + '\n')
+        fp.write(str(self._Size[0]) + ' ' + str(self._Size[1]) + ' ' + str(self._Size[2]) + '\n ')
+        for i in range(self._Size[0]):
+            for j in range(self._Size[1]):
+                for k in range(self._Size[2]):
+                    fp.write(str(data[i][j][k]) + '\n')
+        fp.close()
+
+    def SaveBinaryData(self, filename, data, datatype=' '):
+        latticeparam = self._Struct.Getabc() + self._Struct.GetAlphaBetaGama()
+        with open(filename, 'wb') as outf:
+            outf.write(pack('4i', 3, 0, 0, 0))  # file format version
+            outf.write(pack(
+                '80s',
+                datatype.ljust(80).encode('utf-8')))  # Title 80 characters
+            outf.write(pack('i', 1))  # gType 0 for *.ggrid, 1 for *.pgrid
+            outf.write(pack('i', 0))  # fType 0
+            outf.write(pack('i', 1))  # nVal dummy
+            outf.write(pack('i', 3))  # dimension
+            outf.write(pack('3i', *self._Size))  # numbers of voxels
+            outf.write(pack('i', data.size))  # Total number of voxels
+            outf.write(pack('6f', *latticeparam))  # lattice parameters
+            for k in range(self._Size[2]):
+                for j in range(self._Size[1]):
+                    for i in range(self._Size[0]):
+                        outf.write(pack('f', data[i][j][k]))
+
+    def ReadData(self, filename, data, datatype=' '):
+        fp = open(filename, 'r')
+        datatype = fp.readline()
+        alpha = self._Struct.GetAlphaBetaGama()
+        abc = self._Struct.Getabc()
+        abc = fp.readline().split()
+        alpha = fp.readline().split()
+        strs = fp.readline().split()
+        size = [int(i) for i in strs]
+        if datatype == 'bvs':
+            self.__Data['BVS'] = np.zeros(size)
+            data = self.__Data['BVS']
+        else:
+            self.__Data['BVSE'] = np.zeros(size)
+            data = self.__Data['BVSE']
+        for i in range(size[2]):
+            for j in range(size[1]):
+                for k in range(size[0]):
+                    strs = fp.readline().split()
+                    data[k][j][i] = int(strs[0])
+        fp.close()
+
+    def GetBVSData(self):
+        return self.__Data['BVS']
+
+    def GetBVSEData(self):
+        return self.__Data['BVSE']
+
+    def GetPosSet(self):
+        return self._poss
+
+    def CaluGlobalIndex(self):
+        self.stop = False
+        self._Size.reverse()
+        centrepos = np.zeros(self._Size + [3])
+        self._Data = np.zeros(self._Size, dtype=np.double)
+        for k in range(self._Size[0]):
+            for j in range(self._Size[1]):
+                for i in range(self._Size[2]):
+                    centrepos[k][j][i][2] = k / (self._Size[0] - 1.0)
+                    centrepos[k][j][i][1] = j / (self._Size[1] - 1.0)
+                    centrepos[k][j][i][0] = i / (self._Size[2] - 1.0)
+
+        self._poss = self._Struct.FracPosToCartPos(centrepos)
+        (distance, neighborsindex) = self._Struct.GetKNeighbors(self._poss, kn=8)
+
+        site2atoms = None
+        for k in range(self._Size[0]):
+            for j in range(self._Size[1]):
+                for i in range(self._Size[2]):
+                    if self.stop:
+                        return
+                    
+                    for dindex, index in enumerate(neighborsindex[k][j][i]):
+                        site2 = self._Struct.GetSuperCellusites()[index]
+                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
+                            for key in site2.GetElementsOccupy():
+                                if key != 'Vac':
+                                    site2atoms = key
+                            if self.ValenceOfMoveIon > 0:
+                                key = "".join([self._MoveIon, str(self.ValenceOfMoveIon), site2atoms, str(site2.GetElementsOxiValue()[site2atoms])])
+                            else:
+                                key = "".join([site2atoms, str(site2.GetElementsOxiValue()[site2atoms]), self._MoveIon, str(self.ValenceOfMoveIon)])
+                            if key in self._BVparam:
+                                (r, b) = self._BVparam[key][0]
+                                bv = np.exp((r - distance[k][j][i][dindex]) / b)
+                                self.__Data['BVS'][k][j][i] = self.__Data['BVS'][k][j][i] + bv
+                            else:
+                                print('Not Find bvs param' + key)
+                        else:
+                            pass
+                            # print(site2.GetSiteLabel())
+    
+    def CaluBVSE(self, ProgressCall, Rmin_moveion=3):
+        self.Rmin_moveion = Rmin_moveion
+        
+        if len(self._Struct._OxidationTable) == 0:
+            raise Exception('can not calculate BV and Ea without atom oxi info')
+        
+        self.stop = False
+        
+        centrepos = np.zeros(self._Size + [3])
+        self.__Data['BVS'] = np.zeros(self._Size, dtype=np.double)
+        self.__Data['BVSE'] = np.zeros(self._Size, dtype=np.double)
+        self.__Data['BVEL'] = np.zeros(self._Size, dtype=np.double)
+        
+        for k in range(self._Size[2]):
+            for j in range(self._Size[1]):
+                for i in range(self._Size[0]):
+                    centrepos[i][j][k][2] = k / (self._Size[2] - 1.0)
+                    centrepos[i][j][k][1] = j / (self._Size[1] - 1.0)
+                    centrepos[i][j][k][0] = i / (self._Size[0] - 1.0)
+        
+        if ProgressCall:
+            ProgressCall(0)
+        
+        self._poss = self._Struct.FracPosToCartPos(centrepos)
+
+        atomsq = {}
+        for atom in self._Struct._atomsymbols:
+            atomsq[atom] = 0
+            for site in self._Struct._Sites:
+                if atom in site.GetElements():
+                    key = atom + str(site.GetElementsOxiValue()[atom])
+                    atomsq[atom] = atomsq[atom] + site.GetElementsOxiValue()[atom] * site.GetElementsOccupy()[atom] / math.sqrt(self._Elementsparam[key][3])
+        
+        qsumanion = 0
+        qsumcation = 0
+        for (atom, value) in atomsq.items():
+            if value > 0:
+                qsumcation = qsumcation + value
+            elif value < 0:
+                qsumanion = qsumanion + value
+            else:
+                qsumanion = 0
+                qsumcation = 0
+        
+        qsum = 0.0
+        if self.ValenceOfMoveIon > 0:
+            qsum = -qsumanion / qsumcation
+        else:
+            qsum = -qsumcation / qsumanion
+        
+        key1 = self._MoveIon + str(self.ValenceOfMoveIon)
+        qm1 = self.ValenceOfMoveIon / math.sqrt(self._Elementsparam[key1][3])
+        rm1 = self._Elementsparam[key1][6]
+        
+        ## tqdm color: '#00ff00', 'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white'
+        for i in tqdm(range(self._Size[0]), colour='cyan', desc=None):
+            (distance, neighborsindex) = self._Struct.GetKNeighbors(self._poss[i], kn=128)
+            
+            if ProgressCall:
+                ProgressCall(10 + i * 90 / (self._Size[0] - 1))
+            
+            for j in tqdm(range(self._Size[1]), colour=None, leave=False):
+                
+                ## Single calculation is too fast, not need to use k loop tqdm
+                # for k in tqdm(range(self._Size[2]), colour='black', leave=False):
+                for k in range(self._Size[2]):
+                    
+                    if self.stop:
+                        return False
+                    
+                    bvsdata = 0.0
+                    data = 0.0
+                    cdata = 0.0
+                    bvelcdata = 0.0
+                    N = 0
+                    D0 = 0.0
+                    Rcutoff = 10.0
+                    alpha = 0.0
+                    occupyvalue = 0.0
+                    
+                    list_cdata_Li = []
+                    list_bvelcdata_Li = []
+                    
+                    break_this_point = False
+                    exclude_NN_Li = False
+                    
+                    for dindex, index in enumerate(neighborsindex[j][k]):
+                        if break_this_point:
+                            break
+                        
+                        ## site2 is the neighbor of attempt_Li+
+                        site2 = self._Struct._SuperCellusites[index]
+                        
+                        if site2.GetIronType() * self.ValenceOfMoveIon < 0:
+                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
+                                if ssymbol != 'Vac':
+                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
+                                    if self.ValenceOfMoveIon > 0:
+                                        key = "".join([self._MoveIon, str(self.ValenceOfMoveIon), ssymbol, str(site2oxi)])
+                                    else:
+                                        key = "".join([ssymbol, str(site2oxi), self._MoveIon, str(self.ValenceOfMoveIon)])
+                                    if (key in self._BVSEparam) and (key in self._BVparam):
+                                        (Nc, r0, Rcutoff, D0, Rmin, alpha) = self._BVSEparam[key][0]
+                                        (r, b) = self._BVparam[key][0]
+                                        Rcutoff = 10.0
+                                        if distance[j][k][dindex] <= Rcutoff:
+                                            # bv=np.exp((r0-distance[k][j][i][dindex])*alpha)
+                                            bvs = np.exp((r - distance[j][k][dindex]) / b)
+                                            smin = np.exp((Rmin - distance[j][k][dindex]) * alpha)
+                                            en_s = np.exp((Rmin - Rcutoff) * alpha)
+                                            bvsdata = bvsdata + bvs  #*occupyvalue-((en_s-1)**2-1)
+                                            data = data + ((smin - 1)**2 - 1) * occupyvalue
+                                    else:
+                                        if (key not in self._BVSEparam):
+                                            raise Exception("bvse {0}  param can't find!!!!".format(key))
+                                            ProgressCall(0)
+                                        else:
+                                            raise Exception("bvs {0} param can't find!!!!".format(key))
+                                            ProgressCall(0)
+                        else:
+                            ## When Li+, this if-else is for effect between attempt_Li+ and *cations*
+                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
+                                if ssymbol != 'Vac':
+                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
+                                    
+                                    if ssymbol != self._MoveIon:
+                                        ## For cations around attempt_Li+, which is not Li+
+                                        key = ssymbol + str(site2oxi)
+                                        rm2 = self._Elementsparam[key][6]
+                                        qm2 = site2oxi / math.sqrt(self._Elementsparam[key][3])
+                                        rm1m2 = distance[j][k][dindex]
+                                        f = 0.74
+                                        if rm1m2 > rm2:
+                                            if rm1m2 < Rcutoff:
+                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
+                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
+                                        else:
+                                            ## For rm1m2 <= rm2, this means the sites cation is too close to attempt_Li+
+                                            ## So the calculation of this attempt_Li+ can be breaked
+                                            break_this_point = True
+                                            
+                                            cdata = 300
+                                            bvelcdata = 300
+                                    
+                                    elif ssymbol == self._MoveIon:
+                                        ## For neighbor Li+ around attempt_Li+
+                                        key = ssymbol + str(site2oxi)
+                                        rm2 = self._Elementsparam[key][6]
+                                        qm2 = site2oxi / math.sqrt(self._Elementsparam[key][3])
+                                        rm1m2 = distance[j][k][dindex]
+                                        f = 0.74
+                                        
+                                        R_strict = rm2
+                                        R_strict = self.Rmin_moveion
+                                        # R_strict = 1.45
+                                        if rm1m2 > R_strict:
+                                            if rm1m2 < Rcutoff:
+                                                # cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
+                                                # bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
+                                                
+                                                cdata_Li_i = occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
+                                                bvelcdata_Li_i = occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
+                                                
+                                                list_cdata_Li.append([rm1m2, cdata_Li_i])
+                                                list_bvelcdata_Li.append([rm1m2, bvelcdata_Li_i])
+                                                
+                                        else:
+                                            # cdata = cdata + 0
+                                            # bvelcdata = bvelcdata + 0
+                                            
+                                            pass
+                                    
+                    
+                    list_cdata_Li.sort(key=lambda x: x[0])
+                    list_cdata_Li = list_cdata_Li[1:]
+                    list_bvelcdata_Li.sort(key=lambda x: x[0])
+                    list_bvelcdata_Li = list_bvelcdata_Li[1:]
+                    
+                    cdata += sum([i[1] for i in list_cdata_Li])
+                    bvelcdata += sum([i[1] for i in list_bvelcdata_Li])
+                    
+                    self.__Data['BVSE'][i][j][k] = (0.5 * D0 * (data) + 14.4 * cdata)
+                    self.__Data['BVS'][i][j][k] = bvsdata
+                    self.__Data['BVEL'][i][j][k] = (D0 * (data) + 14.4 * bvelcdata)
+        
+        self.__Data['BVSE'] = self.__Data['BVSE']  #/self.ValenceOfMoveIon
+        self.__Data['BVEL'] = self.__Data['BVEL']  #/self.ValenceOfMoveIon
+        for key, data in self.__Data.items():
+            self.__Max[key] = np.max(data)
+            self.__Min[key] = np.min(data)
+            ashape = self.__Data['BVSE'].shape
+            self.ndata = np.zeros((2 * ashape[0], 2 * ashape[1], 2 * ashape[2]))
+            for i in range(2):
+                for j in range(2):
+                    for k in range(2):
+                        self.ndata[i*ashape[0]:(i+1)*ashape[0], \
+                                                 j*ashape[1]:(j+1)*ashape[1], \
+                                                 k*ashape[2]:(k+1)*ashape[2]]=\
+                                                data-self.__Min[key]
+            self.Ea[key] = self.GetEa(self.ndata)
+
+        _BVSE_Ea = [round(i, 2) for i in self.BVSEEa]
+        print('\nRes {} | Rmin {} | BVSE Ea {}\n'.format(self._reslen, self.Rmin_moveion, _BVSE_Ea))
+        
+        # with open('Ea.txt', 'w') as f:
+            # f.write('Res {} | Rmin {} | BVSE Ea {}\n'.format(self._reslen, self.Rmin_moveion, _BVSE_Ea))
+        
+        return True
+
+    def GetEa(self, data):
+        return [self.GetConnectEa(data,1),\
+                self.GetConnectEa(data,2),\
+                self.GetConnectEa(data,3)]
+
+    def GetConnectEa(self, data, connectnumber):
+        minvalue = 0.0
+        maxvalue = 20.0
+        while (maxvalue - minvalue) > 0.01:
+            testvalue = (maxvalue + minvalue) / 2.0
+            testdata = data < testvalue
+            number = self.CaluRegionConnectivity(testdata)
+            if number >= connectnumber:
+                maxvalue = testvalue
+            else:
+                minvalue = testvalue
+        if maxvalue >= 20.0:
+            return 20000
+        else:
+            return maxvalue
+
+    def CaluRegionConnectivity(self, region):
+        struct = scipy.ndimage.generate_binary_structure(3, 3)
+        lw, num = measurements.label(region, structure=struct)
+        sliced = measurements.find_objects(lw)
+        connectnumber = np.zeros(num, dtype=np.int)
+        if (num > 0):
+            for index, slic in enumerate(sliced):
+                for i in range(len(slic)):
+                    if ((slic[i].start == 0)
+                            and slic[i].stop == region.shape[i]):
+                        connectnumber[index] = connectnumber[index] + 1
+        return np.max(connectnumber)
+
+    # def write_vti_file(self,filename='test.vti'):
+    # imageData = vtk.vtkImageData()
+    # imageData.SetDimensions(self._Size)
+    # self._reslen=0.1
+    # imageData.SetSpacing(self._reslen,self._reslen,self._reslen)
+    # imageData.AllocateScalars(vtk.VTK_FLOAT, 1)
+    # for k in range(self._Size[2]):
+    # for j in range(self._Size[1]):
+    # for i in range(self._Size[0]):
+    # imageData.SetScalarComponentFromDouble(i, j,k, 0, self.__Data['BVSE'][i][j][k])
+    # writer = vtk.vtkXMLImageDataWriter()
+    # writer.SetFileName(filename)
+    # writer.SetInputData(imageData)
+    # writer.Write()
+
+    Data = property(get_data, set_data, del_data, "Data's docstring")
+    Max = property(get_max, set_max, del_max, "Max's docstring")
+    Min = property(get_min, set_min, del_min, "Min's docstring")
+
+
+# if __name__=="__main__":
+#     bvmdata=loadbvparam('bvmparam.data')
+#
+#     print(bvmdata['Na'+'1'+'O'+'-2'])
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVSEParam.dat` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/BVSEParam.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__init__.py` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-# -*- coding: utf-8 -*-
-'''
-modify author: Bowei Pu
-version: 2022.08.17
-note: This is a modified module from BVSE program by Bing He
-function: __init__ class of bvseLi
-'''
-import os
-import time
-from pathlib import Path
-import shutil
-from pickle import NONE
-import ase.io
-from rich.progress import Progress
-
-import bvseLi.Structure as Structure
-import bvseLi.BVAnalysis as BVAnalysis
-import bvseLi.BVAnalysisLi as BVAnalysisLi
-
-
-class Progressbar:
-
-    def __init__(self):
-        self.progress = Progress()
-        self.task = None
-
-    def set_task(self, workstr: str, total):
-        self.task = self.progress.add_task(workstr, total)
-
-    def updatetask(self, i: int):
-        self.progress.update(self.task, advance=0.9)
-        print('    bvse computing  {0:.2f}%'.format(i))
-
-
-def time_used(time0, if_print=False, return_type='tuple'):
-    dt = int(time.time() - time0)
-    h, m, s = dt // 3600, dt // 60 % 60, dt % 60
-    if if_print:
-        print('    time used: {:0>2}h {:0>2}m {:0>2}s'.format(h, m, s))
-        # print('    time used: {:0>2}:{:0>2}:{:0>2}'.format(h, m, s))
-    if return_type.lower() in ['default', 'normal', 'tuple', 'list']:
-        return h, m, s
-    elif return_type.lower() in ['dic']:
-        return {'h': h, 'm': m, 's': s}
-    else:
-        return
-
-
-def time_used_old(time0, if_print=False):
-    dt = time.time() - time0
-    sec = int(dt)
-    mins = round(sec / 60, 2)
-    hour = round(sec / 60 / 60, 2)
-    if if_print:
-        print('    time used: {} h, {} m, {} s'.format(hour, mins, sec))
-    dic = {'h': hour, 'm': mins, 's': sec}
-    return dic
-
-
-class OsPath():
-    '''
-    '''
-    def __init__(self, file):
-        self.file = file
-        
-        self.path = self.abspath = os.path.abspath(self.file)
-        self.parent, self.name = os.path.split(self.abspath)
-        self.dirname, self.basename, self.filename = self.parent, self.name, self.name
-        self.stem, self.suffix = os.path.splitext(self.name)
-        self.path_stem = self.abs_stem = os.path.splitext(self.abspath)[0]
-        
-        self.str = self.string = self.abspath
-        self.posix = self.as_posix()
-    
-    def __str__(self):
-        return self.abspath
-    
-    def __repr__(self):
-        return self.__str__()
-    
-    def __fspath__(self):
-        return self.abspath
-    
-    def absolute(self):
-        return self.abspath
-    
-    def as_posix(self):
-        return Path(self.abspath).as_posix()
-    
-    @staticmethod
-    def get_posix(cls, path):
-        return Path(path).as_posix()
-    
-    def join(self, other: str):
-        return self.__class__(os.path.join(self.abspath, other))
-    
-    def joinpath(self, other: str):
-        return self.join(other)
-    
-    @property
-    def exists(self):
-        return os.path.exists(self.abspath)
-        
-    @property
-    def isfile(self):
-        return os.path.isfile(self.abspath)
-    
-    @property
-    def isdir(self):
-        return os.path.isdir(self.abspath)
-    
-    def rename(self, new_name):
-        return self.__class__(os.path.join(self.dirname, new_name))
-
-
-def bv_calculation(filename,
-                   moveion='Li',
-                   valenceofmoveion=1,
-                   resolution=0.1,
-                   progress=None, 
-                   Rmin_moveion=3, 
-                   engine='bvseLi',
-                   pack_files=True, 
-                   skip_done=True, 
-                   rename_cif=True
-                  ):
-    '''
-    Convenient function to apply BVSELi calculation
-    
-    Args:
-        filename: file path
-        moveion: mobile ion
-        valenceofmoveion: valence of mobile ion
-        resolution: resolution
-        progress: whether desplay progress bar when cal
-        Rmin_moveion: Rmin cutoff to judge whether cal nearby mobile ion
-        engine: choose different bv method. 'bvse' or 'bvseLi'
-        pack_files: if pack output files after calculation
-        skip_done: if skip .cif file which is startswith 'done--'
-        rename_cif: if rename '*.cif' file to 'done--*.cif' after calculation
-    
-    Returns:
-        bvs.Ea['BVSE']
-    
-    Outputs:
-        .npy: Data for numpy load
-        .pgrid: Grid data for VESTA
-        .grd: Grd data
-        INFO.csv: Log to record related info, include filename, res, Rmin, Ea and etc.
-    '''
-    if skip_done:
-        if Path(filename).name.startswith('done--'):
-            return
-    
-    if not progress or progress.lower() in ['default', 'auto']:
-        prgbar = Progressbar()
-        prgbar.set_task('bvse computing progress...', total=100)
-        progress = prgbar.updatetask
-    
-    if engine.lower() in ['default', 'normal', 'bvse']:
-        engine = 'bvse'
-    elif engine.lower() in ['bvseli']:
-        engine = 'bvseli'
-    
-    atoms = ase.io.read(filename, store_tags=True)
-    struc = Structure.Structure()
-    struc.GetAseStructure(atoms)
-    
-    if engine == 'bvse':
-        bvs = BVAnalysis.BVAnalysis()
-        BVMethod = 'BVSE'
-    elif engine == 'bvseli':
-        bvs = BVAnalysisLi.BVAnalysis()
-        BVMethod = 'BVSELi'
-    
-    bvs.SetStructure(struc)
-    bvs.SetMoveIon(moveion)
-    bvs.ValenceOfMoveIon = valenceofmoveion
-    bvs.SetLengthResolution(resolution)
-    
-    time0 = time.time()
-    progress = None
-    if engine == 'bvse':
-        bvs.CaluBVSE(progress)
-    elif engine == 'bvseli':
-        bvs.CaluBVSE(progress, Rmin_moveion)
-    time_info = time_used(time0, if_print=False, return_type='dic')
-    
-    file = OsPath(filename)
-    file_name = Path(filename).name
-    filepath = os.path.abspath(filename)
-    filepath_dire = os.path.split(filepath)[0]
-    filepath_stem = os.path.splitext(filepath)[0]
-    
-    bvs.SaveBVSEData(file.abs_stem)
-    bvs.SaveBVELData(file.abs_stem)
-    bvs.SaveBVSData(file.abs_stem)
-    
-    bv_data = bvs.get_data()
-    bvs.SaveData('{}_BVSELi.grd'.format(file.abs_stem), bv_data['BVSE'], 'BVSE')
-    
-    with open('{}_INFO.csv'.format(file.abs_stem), 'w') as f:
-        f.write('filename,resolution,Rmin_moveion,Ea_BVSE,time_used\n')
-        _BVSE_Ea = [round(i, 2) for i in bvs.BVSEEa]
-        _BVSE_Ea = '[{}]'.format(' '.join([str(i) for i in _BVSE_Ea]))
-        _time_info = '{}h {}m {}s'.format(time_info['h'], time_info['m'], time_info['s'])
-        f.write('{0},{1},{2},{3},{4}'.format(filename, bvs._reslen, bvs.Rmin_moveion, _BVSE_Ea, _time_info))
-    
-    if pack_files:
-        date_short = time.strftime('%y%m%d_%H%M%S')
-        _dire_name = '{}_BVSELi--Res_{}-Rmin_{}--{}'.format(date_short, bvs._reslen, bvs.Rmin_moveion, file.name)
-        _dire = os.path.join(file.dirname, _dire_name)
-        os.mkdir(_dire)
-        shutil.copy2(file.abspath, _dire)
-        for _suffix in ['_BVSELi.npy', 
-                        '_BVSELi.pgrid', 
-                        '_BVELLi.pgrid', 
-                        '_BVSLi.pgrid', 
-                        '_BVSELi.grd', 
-                        '_INFO.csv'
-                       ]:
-            shutil.move('{}{}'.format(file.abs_stem, _suffix), _dire)
-    
-    if rename_cif:
-        file_new = file.rename('done--' + file.name).string
-        os.rename(filename, file_new)
-    
-    return bvs.Ea['BVSE']
-
-
-def bv_calculation_normal(filename,
-                          moveion='Li',
-                          valenceofmoveion=1,
-                          resolution=0.1,
-                          progress='default', 
-                          Rmin_moveion=3
-                         ):
-    
-    prgbar = Progressbar()
-    prgbar.set_task('bvse computing progress...', total=100)
-    if progress in ['default', 'auto']:
-        progress = prgbar.updatetask
-    
-    atoms = ase.io.read(filename, store_tags=True)
-    struc = Structure.Structure()
-    struc.GetAseStructure(atoms)
-    
-    bvs = BVAnalysis.BVAnalysis()
-    bvs.SetStructure(struc)
-    bvs.SetMoveIon(moveion)
-    bvs.ValenceOfMoveIon = valenceofmoveion
-    bvs.SetLengthResolution(resolution)
-    
-    # bvs.CaluBVSE(progress, Rmin_moveion)
-    bvs.CaluBVSE(progress)
-    
-    bvs.SaveBVSEData(os.path.splitext(filename)[0])
-    bv_data = bvs.get_data()
-    bvs.SaveData(os.path.splitext(filename)[0] + '.bvse.grd', bv_data['BVSE'], 'BVSE')
-    
-    return bvs.Ea['BVSE']
-
-
-def bv_calculation_old(filename,
-                   moveion='Li',
-                   valenceofmoveion=1,
-                   resolution=0.1,
-                   progress=None):
-    atoms = ase.io.read(filename, store_tags=True)
-    struc = Structure.Structure()
-    struc.GetAseStructure(atoms)
-    bvs = BVAnalysis.BVAnalysis()
-    bvs.SetStructure(struc)
-    bvs.SetMoveIon(moveion)
-    bvs.ValenceOfMoveIon = valenceofmoveion
-    bvs.SetLengthResolution(resolution)
-    
-    bvs.CaluBVSE(progress)
-    
-    bvs.SaveBVSEData(os.path.splitext(filename)[0])
-    bv_data = bvs.get_data()
-    bvs.SaveData(os.path.splitext(filename)[0] + '.bvse.grd', bv_data['BVSE'], 'BVSE')
-    
-    return bvs.Ea['BVSE']
-    
-    
-    
-    
+# -*- coding: utf-8 -*-
+'''
+modify author: Bowei Pu
+version: 2022.08.17
+note: This is a modified module from BVSE program by Bing He
+function: __init__ class of bvseLi
+'''
+import os
+import time
+from pathlib import Path
+import shutil
+from pickle import NONE
+import ase.io
+from rich.progress import Progress
+
+import bvseLi.Structure as Structure
+import bvseLi.BVAnalysis as BVAnalysis
+import bvseLi.BVAnalysisLi as BVAnalysisLi
+
+
+class Progressbar:
+
+    def __init__(self):
+        self.progress = Progress()
+        self.task = None
+
+    def set_task(self, workstr: str, total):
+        self.task = self.progress.add_task(workstr, total)
+
+    def updatetask(self, i: int):
+        self.progress.update(self.task, advance=0.9)
+        print('    bvse computing  {0:.2f}%'.format(i))
+
+
+def time_used(time0, if_print=False, return_type='tuple'):
+    dt = int(time.time() - time0)
+    h, m, s = dt // 3600, dt // 60 % 60, dt % 60
+    if if_print:
+        print('    time used: {:0>2}h {:0>2}m {:0>2}s'.format(h, m, s))
+        # print('    time used: {:0>2}:{:0>2}:{:0>2}'.format(h, m, s))
+    if return_type.lower() in ['default', 'normal', 'tuple', 'list']:
+        return h, m, s
+    elif return_type.lower() in ['dic']:
+        return {'h': h, 'm': m, 's': s}
+    else:
+        return
+
+
+def time_used_old(time0, if_print=False):
+    dt = time.time() - time0
+    sec = int(dt)
+    mins = round(sec / 60, 2)
+    hour = round(sec / 60 / 60, 2)
+    if if_print:
+        print('    time used: {} h, {} m, {} s'.format(hour, mins, sec))
+    dic = {'h': hour, 'm': mins, 's': sec}
+    return dic
+
+
+class OsPath():
+    '''
+    '''
+    def __init__(self, file):
+        self.file = file
+        
+        self.path = self.abspath = os.path.abspath(self.file)
+        self.parent, self.name = os.path.split(self.abspath)
+        self.dirname, self.basename, self.filename = self.parent, self.name, self.name
+        self.stem, self.suffix = os.path.splitext(self.name)
+        self.path_stem = self.abs_stem = os.path.splitext(self.abspath)[0]
+        
+        self.str = self.string = self.abspath
+        self.posix = self.as_posix()
+    
+    def __str__(self):
+        return self.abspath
+    
+    def __repr__(self):
+        return self.__str__()
+    
+    def __fspath__(self):
+        return self.abspath
+    
+    def absolute(self):
+        return self.abspath
+    
+    def as_posix(self):
+        return Path(self.abspath).as_posix()
+    
+    @staticmethod
+    def get_posix(cls, path):
+        return Path(path).as_posix()
+    
+    def join(self, other: str):
+        return self.__class__(os.path.join(self.abspath, other))
+    
+    def joinpath(self, other: str):
+        return self.join(other)
+    
+    @property
+    def exists(self):
+        return os.path.exists(self.abspath)
+        
+    @property
+    def isfile(self):
+        return os.path.isfile(self.abspath)
+    
+    @property
+    def isdir(self):
+        return os.path.isdir(self.abspath)
+    
+    def rename(self, new_name):
+        return self.__class__(os.path.join(self.dirname, new_name))
+
+
+def bv_calculation(filename,
+                   moveion='Li',
+                   valenceofmoveion=1,
+                   resolution=0.1,
+                   progress=None, 
+                   Rmin_moveion=3, 
+                   engine='bvseLi',
+                   pack_files=True, 
+                   skip_done=True, 
+                   rename_cif=True
+                  ):
+    '''
+    Convenient function to apply BVSELi calculation
+    
+    Args:
+        filename: file path
+        moveion: mobile ion
+        valenceofmoveion: valence of mobile ion
+        resolution: resolution
+        progress: whether desplay progress bar when cal
+        Rmin_moveion: Rmin cutoff to judge whether cal nearby mobile ion
+        engine: choose different bv method. 'bvse' or 'bvseLi'
+        pack_files: if pack output files after calculation
+        skip_done: if skip .cif file which is startswith 'done--'
+        rename_cif: if rename '*.cif' file to 'done--*.cif' after calculation
+    
+    Returns:
+        bvs.Ea['BVSE']
+    
+    Outputs:
+        .npy: Data for numpy load
+        .pgrid: Grid data for VESTA
+        .grd: Grd data
+        INFO.csv: Log to record related info, include filename, res, Rmin, Ea and etc.
+    '''
+    if skip_done:
+        if Path(filename).name.startswith('done--'):
+            return
+    
+    if not progress or progress.lower() in ['default', 'auto']:
+        prgbar = Progressbar()
+        prgbar.set_task('bvse computing progress...', total=100)
+        progress = prgbar.updatetask
+    
+    if engine.lower() in ['default', 'normal', 'bvse']:
+        engine = 'bvse'
+    elif engine.lower() in ['bvseli']:
+        engine = 'bvseli'
+    
+    atoms = ase.io.read(filename, store_tags=True)
+    struc = Structure.Structure()
+    struc.GetAseStructure(atoms)
+    
+    if engine == 'bvse':
+        bvs = BVAnalysis.BVAnalysis()
+        BVMethod = 'BVSE'
+    elif engine == 'bvseli':
+        bvs = BVAnalysisLi.BVAnalysis()
+        BVMethod = 'BVSELi'
+    
+    bvs.SetStructure(struc)
+    bvs.SetMoveIon(moveion)
+    bvs.ValenceOfMoveIon = valenceofmoveion
+    bvs.SetLengthResolution(resolution)
+    
+    time0 = time.time()
+    progress = None
+    if engine == 'bvse':
+        bvs.CaluBVSE(progress)
+    elif engine == 'bvseli':
+        bvs.CaluBVSE(progress, Rmin_moveion)
+    time_info = time_used(time0, if_print=False, return_type='dic')
+    
+    file = OsPath(filename)
+    file_name = Path(filename).name
+    filepath = os.path.abspath(filename)
+    filepath_dire = os.path.split(filepath)[0]
+    filepath_stem = os.path.splitext(filepath)[0]
+    
+    bvs.SaveBVSEData(file.abs_stem)
+    bvs.SaveBVELData(file.abs_stem)
+    bvs.SaveBVSData(file.abs_stem)
+    
+    bv_data = bvs.get_data()
+    bvs.SaveData('{}_BVSELi.grd'.format(file.abs_stem), bv_data['BVSE'], 'BVSE')
+    
+    with open('{}_INFO.csv'.format(file.abs_stem), 'w') as f:
+        f.write('filename,resolution,Rmin_moveion,Ea_BVSE,time_used\n')
+        _BVSE_Ea = [round(i, 2) for i in bvs.BVSEEa]
+        _BVSE_Ea = '[{}]'.format(' '.join([str(i) for i in _BVSE_Ea]))
+        _time_info = '{}h {}m {}s'.format(time_info['h'], time_info['m'], time_info['s'])
+        f.write('{0},{1},{2},{3},{4}'.format(filename, bvs._reslen, bvs.Rmin_moveion, _BVSE_Ea, _time_info))
+    
+    if pack_files:
+        date_short = time.strftime('%y%m%d_%H%M%S')
+        _dire_name = '{}_BVSELi--Res_{}-Rmin_{}--{}'.format(date_short, bvs._reslen, bvs.Rmin_moveion, file.name)
+        _dire = os.path.join(file.dirname, _dire_name)
+        os.mkdir(_dire)
+        shutil.copy2(file.abspath, _dire)
+        for _suffix in ['_BVSELi.npy', 
+                        '_BVSELi.pgrid', 
+                        '_BVELLi.pgrid', 
+                        '_BVSLi.pgrid', 
+                        '_BVSELi.grd', 
+                        '_INFO.csv'
+                       ]:
+            shutil.move('{}{}'.format(file.abs_stem, _suffix), _dire)
+    
+    if rename_cif:
+        file_new = file.rename('done--' + file.name).string
+        os.rename(filename, file_new)
+    
+    return bvs.Ea['BVSE']
+
+
+def bv_calculation_normal(filename,
+                          moveion='Li',
+                          valenceofmoveion=1,
+                          resolution=0.1,
+                          progress='default', 
+                          Rmin_moveion=3
+                         ):
+    
+    prgbar = Progressbar()
+    prgbar.set_task('bvse computing progress...', total=100)
+    if progress in ['default', 'auto']:
+        progress = prgbar.updatetask
+    
+    atoms = ase.io.read(filename, store_tags=True)
+    struc = Structure.Structure()
+    struc.GetAseStructure(atoms)
+    
+    bvs = BVAnalysis.BVAnalysis()
+    bvs.SetStructure(struc)
+    bvs.SetMoveIon(moveion)
+    bvs.ValenceOfMoveIon = valenceofmoveion
+    bvs.SetLengthResolution(resolution)
+    
+    # bvs.CaluBVSE(progress, Rmin_moveion)
+    bvs.CaluBVSE(progress)
+    
+    bvs.SaveBVSEData(os.path.splitext(filename)[0])
+    bv_data = bvs.get_data()
+    bvs.SaveData(os.path.splitext(filename)[0] + '.bvse.grd', bv_data['BVSE'], 'BVSE')
+    
+    return bvs.Ea['BVSE']
+
+
+def bv_calculation_old(filename,
+                   moveion='Li',
+                   valenceofmoveion=1,
+                   resolution=0.1,
+                   progress=None):
+    atoms = ase.io.read(filename, store_tags=True)
+    struc = Structure.Structure()
+    struc.GetAseStructure(atoms)
+    bvs = BVAnalysis.BVAnalysis()
+    bvs.SetStructure(struc)
+    bvs.SetMoveIon(moveion)
+    bvs.ValenceOfMoveIon = valenceofmoveion
+    bvs.SetLengthResolution(resolution)
+    
+    bvs.CaluBVSE(progress)
+    
+    bvs.SaveBVSEData(os.path.splitext(filename)[0])
+    bv_data = bvs.get_data()
+    bvs.SaveData(os.path.splitext(filename)[0] + '.bvse.grd', bv_data['BVSE'], 'BVSE')
+    
+    return bvs.Ea['BVSE']
+    
+    
+    
+
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvse.dat` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/bvse.dat`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,592 +1,592 @@
-cation	cation_valence	anion	anion_valence	Nc	R0	Rcutoff	D0	Rmin	alpha
-Li	1	O	-2	5.021	1.17096	6	0.98816	1.940013	1.937984
-Be	2	O	-2	4	1.20903	5.5	2.768816	1.522169	1.848429
-B	3	O	-2	3.417	1.35761	4.5	2.389237	1.340034	2.597403
-C	4	O	-2	3	1.39826	5	4.791867	1.200889	2.237136
-N	5	O	-2	3	1.46267	5	6.276775	1.161424	2.222222
-Na	1	O	-2	6.52	1.56225	6	0.575227	2.374335	2.293578
-Mg	2	O	-2	5.897	1.48398	5.5	1.575539	1.956265	1.953125
-Al	3	O	-2	5.327	1.59901	5	1.803461	1.758058	2.358491
-Si	4	O	-2	4.1	1.60817	5	2.857198	1.535939	2.314815
-P	5	O	-2	4	1.62038	5	3.896352	1.44066	2.28833
-S	6	O	-2	4	1.6422	5	4.96726	1.381015	2.267574
-Cl	7	O	-2	4	1.67946	5	5.991005	1.348009	2.257336
-K	1	O	-2	8.846	1.94117	6	0.34985	2.766359	2.293578
-Ca	2	O	-2	7.544	1.79519	5.5	0.994291	2.32032	2.10084
-Ga	3	O	-2	4.905	1.71606	5	1.184556	1.79391	2.680965
-Ge	4	O	-2	4.305	1.73939	5	1.913747	1.66872	2.525253
-As	5	O	-2	4.029	1.76689	5	2.719344	1.581273	2.43309
-Se	6	O	-2	4	1.79866	5.5	3.448655	1.532871	2.403846
-Br	7	O	-2	4	1.83658	5.5	4.243387	1.502739	2.364066
-Rb	1	O	-2	10.02	2.08597	6.5	0.268127	2.896827	2.421308
-Sr	2	O	-2	9.4	1.95311	5.5	0.743506	2.535891	2.197802
-In	3	O	-2	6.024	1.90305	5	0.840758	2.024707	2.832861
-Sn	4	O	-2	6.069	1.89019	5	1.352679	1.934221	2.638522
-Sb	5	O	-2	6	1.89768	5.5	1.955227	1.863182	2.5
-Te	6	O	-2	6	1.91343	5.5	2.564057	1.808758	2.427184
-I	7	O	-2	5.8	1.92274	5.5	3.214242	1.741045	2.386635
-Cs	1	O	-2	11.79	2.25899	6.5	0.233071	3.131213	2.386635
-Ba	2	O	-2	10.32	2.15998	6	0.579936	2.737692	2.28833
-Tl	3	O	-2	5.22	2.06297	5	0.676365	2.106422	2.95858
-Pb	4	O	-2	5.74	2.03293	5	1.027186	2.028568	2.824859
-Bi	5	O	-2	6	2.04498	5	1.4405	1.985987	2.695418
-C	2	O	-2	1	1.41368	5	2.405528	1.030976	2.409639
-N	3	O	-2	2	1.40795	5	3.81089	1.137584	2.232143
-P	3	O	-2	3	1.51555	4.5	2.020615	1.410511	2.487562
-S	4	O	-2	3	1.64282	5.5	3.036723	1.411879	2.34192
-As	3	O	-2	3	1.76706	5	1.514929	1.645543	2.475248
-Se	4	O	-2	3	1.80095	5.5	2.380823	1.559575	2.34192
-Sn	2	O	-2	3.325	1.87499	5.5	0.972609	1.964197	2.183406
-Sb	3	O	-2	6	1.92036	5	1.177857	2.075258	2.364066
-Te	4	O	-2	3.396	1.9529	5.5	1.671694	1.752082	2.493766
-I	5	O	-2	3.1	1.97775	6	2.489472	1.644209	2.358491
-Tl	1	O	-2	8.03	1.91752	6	0.349987	2.77086	2.070393
-Pb	2	O	-2	7.541	2.01825	5.5	0.638333	2.441914	2.309469
-Bi	3	O	-2	6.058	2.03677	5.5	0.979037	2.183207	2.415459
-Te	2	O	-2	2	1.39168	6.5	2.626094	1.298928	1.633987
-Sc	3	O	-2	6.255	1.7322	5.5	2.156103	1.996147	2.024291
-Ti	4	O	-2	6	1.72394	5.5	2.813331	1.83144	1.988072
-V	5	O	-2	4.166	1.79445	5.5	3.695335	1.602577	1.960784
-Cr	6	O	-2	4	1.82471	5.5	3.687511	1.532511	2.10084
-Mn	7	O	-2	4	1.87362	6.5	4.916305	1.481714	1.923077
-Fe	3	O	-2	5.733	1.7084	5	1.66681	1.866468	2.380952
-Co	3	O	-2	6	1.59234	5.5	1.870235	1.776198	2.304147
-Ni	2	O	-2	5.933	1.5592	5.5	1.468407	1.924524	2.257336
-Cu	2	O	-2	2.56	1.57422	5	1.853408	1.566333	2.227171
-Zn	2	O	-2	4.718	1.65344	5	1.24031	1.885568	2.48139
-Y	3	O	-2	7.285	1.90384	5.5	1.627011	2.215228	2.09205
-Zr	4	O	-2	6.765	1.84505	5.5	2.191032	1.996025	2.040816
-Nb	5	O	-2	6.044	1.86588	5.5	2.723261	1.854586	2.008032
-Mo	6	O	-2	4.764	1.90934	5	1.991498	1.712544	2.557545
-Tc	7	O	-2	4	1.97036	6	4.041444	1.575183	1.945525
-Ru	6	O	-2	4.5	1.92579	5.5	2.421093	1.664311	2.352941
-Rh	4	O	-2	6	1.77675	5.5	1.627252	1.817932	2.48139
-Pd	2	O	-2	4	1.62359	5.5	1.739103	1.836711	2.008032
-Ag	1	O	-2	4.438	1.78239	5	0.635187	2.225785	2.538071
-Cd	2	O	-2	6.176	1.83926	5.5	0.983461	2.169398	2.457002
-Lu	3	O	-2	6.83	1.91728	5.5	1.194883	2.136	2.375297
-Hf	4	O	-2	7.105	1.83361	6	1.89992	1.999643	2.09205
-Ta	5	O	-2	6.09	1.86816	5.5	2.366685	1.85532	2.057613
-W	6	O	-2	5.688	1.90641	5	1.842666	1.777132	2.493766
-Re	7	O	-2	4.098	1.97792	6	3.555929	1.596339	1.968504
-Os	8	O	-2	5.333	1.97728	6	3.710191	1.661463	1.953125
-Ir	5	O	-2	6	1.89791	6	2.324762	1.83476	2.087683
-Pt	2	O	-2	4	1.51205	5.5	2.149986	1.801793	1.74216
-Au	3	O	-2	4	1.81761	5.5	1.969672	1.813123	2.008032
-Hg	2	O	-2	6.966	1.81276	5.5	1.128521	2.252751	2.150538
-La	3	O	-2	9.83	2.06392	5.5	1.185874	2.469886	2.217295
-Ce	4	O	-2	7.867	2.02821	5.5	1.484118	2.198725	2.257336
-Pr	3	O	-2	9.067	2.03652	5.5	1.170407	2.371126	2.277904
-Nd	3	O	-2	8.647	2.02425	5.5	1.132045	2.330162	2.336449
-Ti	3	O	-2	6	1.69766	5.5	1.978506	1.886194	2.173913
-V	4	O	-2	5.738	1.74932	5	2.080473	1.776375	2.347418
-Cr	4	O	-2	5.429	1.76095	5.5	1.933285	1.76209	2.444988
-Mn	6	O	-2	4	1.82018	5.5	2.822364	1.529314	2.403846
-Fe	2	O	-2	5.743	1.57911	5.5	1.692689	1.960053	2.083333
-Co	4	O	-2	4	1.79444	5.5	2.358037	1.679593	2.267574
-Ni	4	O	-2	6	1.72159	5	1.864513	1.765079	2.487562
-Cu	3	O	-2	4	1.70964	5	1.882423	1.708232	2.34192
-Nb	4	O	-2	6	1.78543	6	2.709602	1.859895	1.901141
-Mo	5	O	-2	5.98	1.8476	5.5	2.648016	1.786697	2.074689
-Ru	5	O	-2	6	1.87442	5.5	2.132078	1.815714	2.293578
-Rh	3	O	-2	6	1.67013	5.5	1.928259	1.869147	2.09205
-Pd	4	O	-2	5.333	1.805	5.5	2.042177	1.798133	2.227171
-Ag	3	O	-2	6.25	1.84687	5.5	1.52826	2.0348	2.252252
-Ta	4	O	-2	5.5	1.75632	6	2.756548	1.798256	1.831502
-W	5	O	-2	6	1.81975	6	2.615701	1.762615	2.008032
-Re	6	O	-2	5.5	1.91007	6	2.950986	1.711469	2.008032
-Os	7	O	-2	6	1.95775	5.5	2.919483	1.728686	2.087683
-Ir	4	O	-2	6	1.83233	5.5	1.686674	1.874017	2.293578
-Hg	1	O	-2	4.786	1.8128	5.5	0.739306	2.431553	2.150538
-V	3	O	-2	6	1.67799	5.5	1.82936	1.857967	2.277904
-Cr	3	O	-2	6	1.66198	5.5	1.773346	1.838872	2.325581
-Mn	5	O	-2	4	1.78879	5.5	2.464555	1.575774	2.421308
-Fe	4	O	-2	6	1.76559	5.5	1.872848	1.827859	2.439024
-Co	2	O	-2	5.506	1.59773	5.5	1.514761	1.933621	2.217295
-Ni	3	O	-2	6	1.64888	5.5	1.661905	1.818873	2.415459
-Cu	1	O	-2	2.56	1.5873	5	0.664171	1.782692	2.932551
-Nb	3	O	-2	6	1.74581	6	2.028483	1.951898	1.996008
-Mo	4	O	-2	6	1.7239	6.5	3.108069	1.850992	1.779359
-Ru	4	O	-2	6	1.79363	5.5	1.995133	1.840532	2.227171
-Ag	2	O	-2	5	1.72209	5.5	1.583396	2.041706	1.996008
-W	4	O	-2	6	1.74558	6	2.471141	1.819454	1.923077
-Re	5	O	-2	6	1.82664	6	2.41099	1.769141	2.087683
-Os	6	O	-2	6	1.93192	5.5	2.448709	1.782799	2.159827
-Pt	4	O	-2	6	1.82198	5.5	2.038254	1.871736	2.087683
-Au	1	O	-2	2	1.71819	5.5	0.853044	1.895429	2.267574
-V	2	O	-2	6	1.59976	5.5	1.640237	1.997526	2.096436
-Cr	2	O	-2	5.6	1.59356	5.5	1.691613	1.961299	2.083333
-Mn	4	O	-2	5.923	1.73272	5	1.858861	1.770446	2.487562
-Co	1	O	-2	2	1.29501	5.5	2.393481	1.640592	1.610306
-Mo	3	O	-2	5.7	1.78933	5.5	1.428262	1.929735	2.392344
-Ru	3	O	-2	6	1.72066	5.5	1.540613	1.8932	2.325581
-Re	4	O	-2	6	1.78237	6	2.316639	1.844971	1.972387
-Pt	3	O	-2	5	1.66559	5.5	2.359527	1.819377	1.831502
-Cr	5	O	-2	4	1.76781	5.5	2.365511	1.555463	2.487562
-Mn	3	O	-2	5.862	1.68993	5.5	1.812832	1.857862	2.28833
-Os	4	O	-2	6	1.75302	6	2.27524	1.812439	2.008032
-Mn	2	O	-2	5.91	1.62758	5.5	1.641434	2.029688	2.079002
-Ce	3	O	-2	9.147	2.03118	5.5	1.220483	2.37861	2.227171
-Sm	3	O	-2	8.119	2.01168	5.5	1.176217	2.295359	2.309469
-Eu	3	O	-2	7.743	2.00469	5.5	1.195447	2.268881	2.304147
-Gd	3	O	-2	8.052	1.99654	5.5	1.091613	2.271904	2.409639
-Tb	3	O	-2	7.958	1.95675	5.5	1.20764	2.235634	2.309469
-Dy	3	O	-2	7.828	1.96029	5.5	1.173498	2.226892	2.347418
-Ho	3	O	-2	7.5	1.97099	5.5	1.121573	2.211215	2.409639
-Er	3	O	-2	7.135	1.95608	5.5	1.123941	2.174771	2.427184
-Tm	3	O	-2	6.912	1.94901	5.5	1.181379	2.160417	2.375297
-Yb	3	O	-2	6.875	1.92872	5.5	1.219894	2.142197	2.347418
-Yb	2	O	-2	8	1.63254	5.5	1.384137	2.209419	1.960784
-Eu	2	O	-2	10.111	1.89158	6	1.130318	2.538459	2.024291
-Tb	4	O	-2	6	1.96244	6	1.701319	2.385063	2.024291
-Th	4	O	-2	8.941	2.04983	6	1.573737	2.310462	2.057613
-U	6	O	-2	6.987	2.02317	6	2.627524	1.992868	1.897533
-Cl	5	O	-2	3	1.69552	5.5	4.290893	1.356529	2.247191
-Cl	3	O	-2	2	1.72265	5.5	3.071187	1.384411	2.03666
-Li	1	S	-2	4.604	1.46652	6	1.04027  	2.40971 	1.531394
-#Be	2	S	-2	4	1.5784	6.5	5.102614	1.056091	-1.477105
-B	3	S	-2	3.417	1.78195	6	3.21881	1.798962	1.745201
-C	4	S	-2	3	1.84354	6	4.870252	1.618649	1.727116
-Na	1	S	-2	6.52	1.83088	6.5	0.630673	2.916205	1.615509
-Mg	2	S	-2	5.897	1.82372	6.5	1.645364	2.457529	1.540832
-Al	3	S	-2	5.327	2.05965	6	1.891546	2.302878	1.818182
-Si	4	S	-2	4.1	2.09975	6.5	2.948361	2.042192	1.785714
-P	5	S	-2	4	2.14917	6	3.939695	1.951558	1.766784
-S	6	S	-2	4	2.2	5.5	4.950597	1.896737	1.751313
-K	1	S	-2	8.846	2.16803	6.5	0.41168	3.315285	1.745201
-Ca	2	S	-2	7.544	2.11148	7	1.098221	2.835405	1.633987
-Ga	3	S	-2	4.905	2.12458	6	1.282374	2.268677	2.070393
-Ge	4	S	-2	4.305	2.19183	6	2.050539	2.142348	1.945525
-As	5	S	-2	4.029	2.27986	6.5	2.850033	2.079575	1.872659
-Rb	1	S	-2	10.02	2.30817	6.5	0.325038	3.460253	1.818182
-Sr	2	S	-2	9.4	2.26765	7	0.842963	3.081154	1.692047
-In	3	S	-2	6.024	2.30797	6	0.92204	2.515464	2.192982
-Sn	4	S	-2	6.069	2.36256	6	1.459465	2.466684	2.03252
-Sb	5	S	-2	6	2.44254	6	2.058532	2.441945	1.923077
-Cs	1	S	-2	11.79	2.52283	6.5	0.249303	3.667187	1.926782
-Ba	2	S	-2	10.32	2.44239	7	0.682017	3.267913	1.745201
-P	3	S	-2	3	1.96089	6	2.224943	1.859402	1.865672
-As	3	S	-2	3	2.20841	6	1.735537	2.095302	1.851852
-Sn	2	S	-2	3.325	2.32497	6	0.701776	2.431194	2.087683
-Sb	3	S	-2	6	2.36947	6	1.138983	2.597379	1.941748
-Tl	1	S	-2	8.03	2.3826	6	0.2208	3.182358	2.197802
-Pb	2	S	-2	7.541	2.38758	6	0.567913	2.905146	2.028398
-Bi	3	S	-2	6.058	2.41824	6.5	1.048372	2.656656	1.912046
-Sc	3	S	-2	6.255	2.0945	7	2.316425	2.475159	1.584786
-Ti	4	S	-2	6	2.17452	7	2.897523	2.350525	1.5625
-V	5	S	-2	4.166	2.29252	7	3.726229	2.088459	1.545595
-#Cr	6	S	-2	4	2.103	6.5	3.780483	2.289947	-1.533742
-Ni	2	S	-2	5.933	1.85695	5.5	1.253997	2.288097	2.024291
-Cu	2	S	-2	2.56	1.94997	6	1.430321	1.957596	2.04918
-Zn	2	S	-2	4.718	1.94373	6	1.485755	2.307582	1.851852
-Y	3	S	-2	7.285	2.25923	7	1.797063	2.710781	1.626016
-Zr	4	S	-2	6.765	2.26265	7	2.330585	2.500694	1.597444
-#Mo	6	S	-2	4.764	2.187	6.5	3.324576	2.251139	-1.560062
-Pd	2	S	-2	4	2.02559	5.5	0.921219	2.200028	2.277904
-Ag	1	S	-2	4.438	2.11006	5	0.392994	2.520847	2.739726
-Cd	2	S	-2	6.176	2.12789	5.5	1.13392	2.614981	1.883239
-Lu	3	S	-2	6.83	2.28119	7	1.388246	2.627609	1.795332
-Hf	4	S	-2	7.105	2.2355	7	2.057539	2.495677	1.626016
-Ta	5	S	-2	6.09	2.2786	6.5	2.543639	2.308695	1.607717
-Pt	2	S	-2	4	2.0245	5.5	0.845436	2.178404	2.283105
-Hg	2	S	-2	6.966	2.20501	5.5	0.806433	2.66333	2.114165
-La	3	S	-2	9.83	2.4033	6.5	1.358302	2.992782	1.70068
-Pr	3	S	-2	9.067	2.46496	6	1.017448	2.877435	2.004008
-Nd	3	S	-2	8.647	2.44624	6	1.072575	2.851212	1.960784
-Ti	3	S	-2	6	2.11813	6	1.415711	2.32404	2.09205
-V	4	S	-2	5.738	2.1676	6.5	1.951626	2.233445	1.953125
-Fe	2	S	-2	5.743	2.01111	5.5	1.036628	2.368789	2.188184
-Nb	4	S	-2	6	2.28012	5.5	1.101045	2.2928	2.427184
-Ta	4	S	-2	5.5	2.28935	5.5	1.010309	2.258914	2.439024
-V	3	S	-2	6	2.02622	6.5	1.588277	2.25755	2.004008
-Cr	3	S	-2	6	2.04397	5.5	1.627769	2.282954	1.968504
-Co	2	S	-2	5.506	1.99705	5.5	1.174488	2.374249	2.053388
-Ni	3	S	-2	6	1.95763	5.5	1.777739	2.215633	1.912046
-Cu	1	S	-2	2.56	1.80744	5	0.704448	2.08186	2.380952
-W	4	S	-2	6	2.22672	6	1.050809	2.246646	2.398082
-Pt	4	S	-2	6	2.19999	6	1.265783	2.249872	2.183406
-Au	1	S	-2	2	2.06404	4.5	0.368405	2.155176	2.923977
-V	2	S	-2	6	1.89815	6	1.092053	2.288101	2.169197
-Cr	2	S	-2	5.6	1.9093	5.5	1.089919	2.262838	2.183406
-Mn	4	S	-2	5.923	2.30057	6	1.997166	2.391923	1.865672
-Mo	3	S	-2	5.7	2.06172	6	1.519179	2.283669	1.926782
-Re	4	S	-2	6	2.268	6	1.098995	2.294802	2.320186
-Mo	2	S	-2	5.5	2.07169	5.5	0.797065	2.349596	2.369668
-Mn	2	S	-2	5.91	2.15468	5.5	0.783125	2.474786	2.463054
-Re	3	S	-2	6	2.2071	6	0.810667	2.332185	2.493766
-Ce	3	S	-2	9.147	2.50404	6	0.968018	2.904365	2.04499
-Sm	3	S	-2	8.119	2.4146	6	1.077495	2.782816	1.980198
-Eu	3	S	-2	7.743	2.39179	6	1.087691	2.734937	1.988072
-Gd	3	S	-2	8.052	2.37028	6	1.280701	2.797353	1.811594
-Tb	3	S	-2	7.958	2.36384	6	1.100521	2.724591	1.980198
-Dy	3	S	-2	7.828	2.34124	6	1.13993	2.703826	1.953125
-Ho	3	S	-2	7.5	2.33798	6	1.190448	2.691208	1.915709
-Er	3	S	-2	7.135	2.32366	6	1.220568	2.655055	1.904762
-Tm	3	S	-2	6.912	2.3107	6	1.196692	2.615977	1.937984
-Yb	3	S	-2	6.875	2.31245	6	1.176666	2.609189	1.956947
-Yb	2	S	-2	8	2.40079	6	0.617429	2.834914	2.34192
-Eu	2	S	-2	10.111	2.47173	6	0.621323	3.032226	2.257336
-Th	4	S	-2	8.941	2.45709	7	1.499684	2.809767	1.727116
-Li	1	Se	-2	5.118	1.62021	7	0.88750 	2.68386 	1.461988
-#Be	2	Se	-2	4	1.7043	7	4.388588	1.163025	-1.412429
-#B	3	Se	-2	3.417	1.9187	6	3.152102	1.785319	-1.647446
-Na	1	Se	-2	6.52	1.8988	7	0.576407	3.046979	1.538462
-#Mg	2	Se	-2	5.897	1.7043	7	4.725019	0.881992	-1.412429
-Al	3	Se	-2	5.327	2.17392	6.5	1.73113	2.440109	1.718213
-Si	4	Se	-2	4.1	2.23551	5.5	2.133055	2.181429	1.890359
-P	5	Se	-2	4	2.43695	7	3.352569	2.231858	1.666667
-K	1	Se	-2	8.846	2.29712	7	0.373639	3.51499	1.655629
-Ca	2	Se	-2	7.544	2.20285	7	1.001348	2.972826	1.55521
-Ga	3	Se	-2	4.905	2.24723	6.5	1.179547	2.40959	1.949318
-Ge	4	Se	-2	4.305	2.33264	6	1.868512	2.289073	1.834862
-Rb	1	Se	-2	10.02	2.40364	7	0.298431	3.629609	1.724138
-Sr	2	Se	-2	9.4	2.36718	7	0.770499	3.2336	1.607717
-In	3	Se	-2	6.024	2.43051	6	0.85029	2.661292	2.066116
-Sn	4	Se	-2	6.069	2.50725	6	1.335624	2.62763	1.915709
-Sb	5	Se	-2	6	2.58978	7	1.880426	2.599348	1.814882
-Cs	1	Se	-2	11.79	2.64858	7	0.229573	3.87313	1.818182
-Ba	2	Se	-2	10.32	2.51975	7	0.712287	3.476334	1.540832
-As	3	Se	-2	3	2.34035	6.5	1.579204	2.229757	1.751313
-Sb	3	Se	-2	6	2.47586	6.5	1.055133	2.729272	1.831502
-Tl	1	Se	-2	8.03	2.39935	6.5	0.228618	3.317982	1.968504
-Pb	2	Se	-2	7.541	2.46755	6.5	0.532474	3.031456	1.908397
-Bi	3	Se	-2	6.058	2.54545	7	0.963506	2.808944	1.805054
-#Cr	6	Se	-2	4	2.3	7	3.289049	2.501378	-1.464129
-Ni	2	Se	-2	5.933	1.89863	6	1.184866	2.368628	1.904762
-Cu	2	Se	-2	2.56	2.02888	6	1.339462	2.047631	1.926782
-Zn	2	Se	-2	4.718	2.00075	6	1.385461	2.396213	1.751313
-#Mo	6	Se	-2	4.764	2.3824	6.5	2.900851	2.455649	-1.488095
-Pd	2	Se	-2	4	2.13063	6	0.867507	2.328957	2.123142
-Ag	1	Se	-2	4.438	2.17409	5	0.364436	2.619255	2.597403
-Cd	2	Se	-2	6.176	2.16209	6.5	1.065618	2.689779	1.782531
-Hf	4	Se	-2	7.105	2.37893	7.5	1.839029	2.659792	1.550388
-Ta	5	Se	-2	6.09	2.51263	7	2.205338	2.549483	1.529052
-Pt	2	Se	-2	4	2.16525	6	0.599859	2.295839	2.457002
-Hg	2	Se	-2	6.966	2.25179	6	0.766574	2.754918	1.984127
-Pr	3	Se	-2	9.067	2.52676	7	0.956529	2.978932	1.890359
-Pd	4	Se	-2	5.333	2.31115	6.5	1.490694	2.336285	1.923077
-Ta	4	Se	-2	5.5	2.36128	6	0.895197	2.338963	2.369668
-V	3	Se	-2	6	2.13686	6.5	1.464549	2.391889	1.886792
-Cr	3	Se	-2	6	2.14649	6	1.503457	2.409792	1.855288
-Co	2	Se	-2	5.506	2.10951	6	1.084223	2.519929	1.930502
-Cu	1	Se	-2	2.56	1.89561	5.5	0.665431	2.200809	2.217295
-Pt	4	Se	-2	6	2.30943	6	1.184141	2.374275	2.04499
-Au	1	Se	-2	2	2.17613	4	0.309936	2.270736	2.890173
-Mn	2	Se	-2	5.91	2.24751	5.5	0.727927	2.598448	2.320186
-Ce	3	Se	-2	9.147	2.52663	7	0.92697	2.970218	1.923077
-Er	3	Se	-2	7.135	2.4342	7	1.125706	2.796224	1.798561
-Yb	3	Se	-2	6.875	2.42113	7	1.088819	2.7472	1.845018
-Yb	2	Se	-2	8	2.62618	7	0.562768	3.098868	2.183406
-Th	4	Se	-2	8.941	2.5485	7.5	1.385614	2.932808	1.636661
-Li	1	Te	-2	4.333	1.71028	7	0.88544 	2.73313 	1.371742
-#Be	2	Te	-2	4	1.8497	7	4.022722	1.283697	-1.328021
-#B	3	Te	-2	3.417	2.0982	6.5	3.018917	1.965185	-1.517451
-Na	1	Te	-2	6.52	2.03011	7	0.549276	3.269608	1.438849
-#Mg	2	Te	-2	5.897	1.9497	7	2.962016	1.160853	-1.470588
-Al	3	Te	-2	5.327	2.38658	7	1.657011	2.688729	1.582278
-K	1	Te	-2	8.846	2.41802	7	0.362353	3.742871	1.540832
-#Ca	2	Te	-2	7.544	2.3886	7	2.188266	1.397063	-1.451379
-Ga	3	Te	-2	4.905	2.44491	7	1.141133	2.63573	1.792115
-Ge	4	Te	-2	4.305	2.57461	7	1.782504	2.540892	1.686341
-Rb	1	Te	-2	10.02	2.43463	7.5	0.298622	3.779363	1.597444
-#Sr	2	Te	-2	9.4	2.5405	7	1.812178	1.418321	-1.497006
-In	3	Te	-2	6.024	2.62278	6.5	0.850959	2.89526	1.872659
-Sn	4	Te	-2	6.069	2.73112	7	1.291437	2.877902	1.760563
-Cs	1	Te	-2	11.79	2.78226	7.5	0.225509	4.127357	1.680672
-Ba	2	Te	-2	10.32	2.68807	7	0.606266	3.65307	1.540832
-Ge	2	Te	-2	4.305	2.26937	7	0.842876	2.614722	1.709402
-As	3	Te	-2	3	2.48812	7	1.536863	2.385037	1.623377
-Sb	3	Te	-2	6	2.73139	7	0.9996	3.018997	1.692047
-Tl	1	Te	-2	8.03	2.50518	6	0.213006	3.480158	1.883239
-Bi	3	Te	-2	6.058	2.82304	7	0.906776	3.120878	1.669449
-Ti	4	Te	-2	6	2.41793	7.5	2.501975	2.639068	1.396648
-Cr	6	Te	-2	4	2.609	8	3.737637	2.242906	1.371742
-Ni	2	Te	-2	5.933	2.11175	6.5	1.127862	2.632744	1.751313
-Zn	2	Te	-2	4.718	2.15126	7	1.333912	2.590758	1.623377
-#Mo	6	Te	-2	4.764	2.66	6.5	2.637957	2.749595	-1.3947
-Ag	1	Te	-2	4.438	2.34487	5	0.357046	2.845751	2.380952
-Cd	2	Te	-2	6.176	2.36683	7	1.017319	2.950242	1.647446
-Ta	5	Te	-2	6.09	2.71824	7	2.072226	2.772261	1.430615
-Hg	2	Te	-2	6.966	2.37917	7	0.760988	2.945194	1.821494
-Cr	3	Te	-2	6	2.30242	6.5	1.461856	2.602311	1.712329
-Cu	1	Te	-2	2.56	1.89529	6	0.70548	2.254788	2.012072
-Cr	2	Te	-2	5.6	2.18257	6.5	0.991672	2.618827	1.872659
-Nb	2	Te	-2	6	2.39087	6	0.598344	2.732389	2.232143
-Ta	2	Te	-2	6	2.20689	6	0.966348	2.705968	1.686341
-Mn	2	Te	-2	5.91	2.43113	6	0.71114	2.829003	2.12766
-Sm	3	Te	-2	8.119	2.71979	7	0.968805	3.173281	1.72117
-Li	1	F	-1	5.289	1.08674	6	0.49611 	1.87265 	1.968504
-Be	2	F	-1	4	1.14986	5.5	1.39717	1.4585	1.879699
-B	3	F	-1	3.417	1.19909	5	2.625262	1.208508	1.845018
-C	4	F	-1	3	1.37249	6	3.759427	1.146081	1.828154
-N	5	F	-1	3	1.40717	6	5.156374	1.055975	1.818182
-Na	1	F	-1	6.52	1.42885	5.5	0.295862	2.232158	2.109705
-Mg	2	F	-1	5.897	1.40956	5.5	0.796133	1.875696	1.984127
-Al	3	F	-1	5.327	1.4197	5.5	1.447303	1.64117	1.926782
-Si	4	F	-1	4.1	1.45654	5.5	2.362172	1.39289	1.890359
-P	5	F	-1	4	1.4761	7	3.28597	1.280179	1.869159
-S	6	F	-1	4	1.55	5	2.655352	1.291705	2.267574
-K	1	F	-1	8.846	1.83331	5.5	0.176234	2.645968	2.336449
-Ca	2	F	-1	7.544	1.71038	5.5	0.498644	2.226693	2.141328
-Ga	3	F	-1	4.905	1.56039	5.5	0.922174	1.684414	2.217295
-Ge	4	F	-1	4.305	1.57864	5.5	1.567311	1.521889	2.066116
-As	5	F	-1	4.029	1.60379	6	2.291271	1.405455	1.988072
-Rb	1	F	-1	10.02	1.99137	5.5	0.133404	2.785647	2.475248
-Sr	2	F	-1	9.4	1.86817	5.5	0.371198	2.440209	2.242152
-In	3	F	-1	6.024	1.75728	5.5	0.626012	1.933906	2.375297
-Sn	4	F	-1	6.069	1.75558	5.5	1.051935	1.839948	2.169197
-Sb	5	F	-1	6	1.76603	6	1.552674	1.753234	2.04499
-Xe	6	F	-1	4	1.86157	6	1.621152	1.565362	2.320186
-Cs	1	F	-1	11.79	2.15318	6	0.12472	3.052764	2.336449
-Ba	2	F	-1	10.32	2.06475	6	0.289369	2.631527	2.336449
-Tl	3	F	-1	5.22	1.857	5.5	0.345633	1.905526	3.076923
-Pb	4	F	-1	5.74	1.93428	5.5	0.76278	1.959449	2.358491
-Bi	5	F	-1	6	1.86984	5.5	1.137508	1.833638	2.232143
-As	3	F	-1	3	1.683	5	0.804158	1.565379	2.463054
-Sb	3	F	-1	6	1.83448	5.5	0.634722	1.999054	2.320186
-Xe	4	F	-1	4	1.85567	6.5	1.488549	1.712146	1.890359
-Tl	1	F	-1	8.03	1.82737	6	0.185412	2.702515	2.03666
-Pb	2	F	-1	7.541	1.90916	6	0.360632	2.365394	2.207506
-Bi	3	F	-1	6.058	1.93046	5.5	0.53418	2.088603	2.364066
-Xe	2	F	-1	4	1.77407	6.5	0.722521	2.0405	1.757469
-Sc	3	F	-1	6.255	1.65325	6	1.533224	1.913247	2.061856
-Ti	4	F	-1	6	1.6617	5.5	1.659907	1.748926	2.227171
-Fe	3	F	-1	5.733	1.63674	5	1.175592	1.791926	2.43309
-Co	3	F	-1	6	1.56345	5.5	1.395376	1.753918	2.257336
-Ni	2	F	-1	5.933	1.49655	5	1.10969	1.874661	2.212389
-Cu	2	F	-1	2.56	1.4953	5.5	1.423726	1.493666	2.188184
-Zn	2	F	-1	4.718	1.57447	5	0.925848	1.812843	2.463054
-Y	3	F	-1	7.285	1.89262	5.5	0.757641	2.11472	2.638522
-Zr	4	F	-1	6.765	1.83174	5.5	1.005776	1.927834	2.57732
-Nb	5	F	-1	6.044	1.76034	5.5	1.966109	1.751349	2.04499
-Rh	4	F	-1	6	1.68686	5.5	1.224679	1.733553	2.463054
-Pd	2	F	-1	4	1.56885	5.5	1.299983	1.793725	1.976285
-Ag	1	F	-1	4.438	1.58298	5	0.727114	2.196512	2.008032
-Cd	2	F	-1	6.176	1.73948	5.5	0.755986	2.084803	2.403846
-Lu	3	F	-1	6.83	1.80738	5.5	0.853953	2.023989	2.427184
-Hf	4	F	-1	7.105	1.7752	5.5	1.334791	1.937534	2.132196
-Ta	5	F	-1	6.09	1.79011	5.5	1.682167	1.778032	2.096436
-Au	3	F	-1	4	1.697	5.5	1.533484	1.706806	1.972387
-Hg	2	F	-1	6.966	1.7338	5.5	0.850135	2.187943	2.114165
-La	3	F	-1	9.83	1.96577	5.5	0.844511	2.366189	2.257336
-Pr	3	F	-1	9.067	1.91752	5.5	0.900775	2.268753	2.232143
-Nd	3	F	-1	8.647	1.91099	5.5	0.870992	2.232524	2.28833
-Ti	3	F	-1	6	1.6318	5.5	1.493295	1.829107	2.136752
-Cr	4	F	-1	5.429	1.64899	5	1.516679	1.658904	2.392344
-Fe	2	F	-1	5.743	1.50766	5.5	1.280077	1.902081	2.04499
-Ni	4	F	-1	6	1.61746	5.5	1.45655	1.670016	2.43309
-Cu	3	F	-1	4	1.54272	5.5	1.531932	1.554592	2.28833
-Nb	4	F	-1	6	1.75844	6	1.995819	1.840216	1.872659
-Ru	5	F	-1	6	1.77634	5.5	1.653541	1.724517	2.247191
-Rh	3	F	-1	6	1.63692	5.5	1.440772	1.843667	2.04918
-Pd	4	F	-1	5.333	1.68582	5.5	1.59323	1.688346	2.188184
-Ag	3	F	-1	6.25	1.71485	5.5	1.189009	1.916593	2.212389
-Pt	5	F	-1	6	1.78573	5.5	1.362673	1.734251	2.358491
-Hg	1	F	-1	4.786	1.76507	5.5	0.547747	2.401203	2.114165
-V	3	F	-1	6	1.61581	5.5	1.386802	1.804823	2.232143
-Cr	3	F	-1	6	1.58975	5.5	1.347343	1.775673	2.283105
-Co	2	F	-1	5.506	1.51442	5.5	1.155873	1.86403	2.173913
-Ni	3	F	-1	6	1.56869	5	1.275911	1.748854	2.364066
-Ag	2	F	-1	5	1.6378	5.5	1.195671	1.973406	1.964637
-Ta	3	F	-1	6	1.52314	6	1.747189	1.79512	1.801802
-Pt	4	F	-1	6	1.69132	5.5	1.597082	1.753192	2.04918
-V	2	F	-1	6	1.53303	5.5	1.232616	1.943136	2.061856
-Cr	2	F	-1	5.6	1.54102	5.5	1.26782	1.920471	2.04499
-Mn	4	F	-1	5.923	1.61606	5	1.45541	1.663202	2.439024
-Mo	3	F	-1	5.7	1.73819	5.5	1.078285	1.886081	2.34192
-Os	5	F	-1	6	1.75815	6	1.83525	1.705754	2.04918
-Mn	3	F	-1	5.862	1.59633	5.5	1.397213	1.775416	2.242152
-Mn	2	F	-1	5.91	1.56491	5.5	1.16586	1.962266	2.109705
-Ce	3	F	-1	9.147	1.92656	5.5	0.932803	2.289753	2.183406
-Sm	3	F	-1	8.119	1.88844	5.5	0.905474	2.187001	2.267574
-Eu	3	F	-1	7.743	1.87763	5.5	0.92616	2.15759	2.257336
-Gd	3	F	-1	8.052	1.90718	5.5	0.770786	2.177537	2.463054
-Tb	3	F	-1	7.958	1.83798	5.5	0.932919	2.132299	2.262443
-#Dy	3	F	-1	7.828	1.85	5.5	1.485846	1.296738	-2.298851
-Ho	3	F	-1	7.5	1.84485	5.5	0.871595	2.100218	2.358491
-Er	3	F	-1	7.135	1.84663	5.5	0.868164	2.078788	2.375297
-Tm	3	F	-1	6.912	1.81795	5.5	0.920982	2.044246	2.325581
-Yb	3	F	-1	6.875	1.80974	5.5	0.945748	2.037278	2.298851
-Eu	2	F	-1	10.111	1.8142	5.5	0.847162	2.482968	1.988072
-Th	4	F	-1	8.941	2.40121	7	1.270178	2.697147	1.782531
-Li	1	Cl	-1	5.258	1.39892	7	0.49302 	2.39647 	1.577287
-Be	2	Cl	-1	4	1.52729	6.5	1.323436	1.9291	1.517451
-#B	3	Cl	-1	3.417	1.675	6	2.579816	1.529824	-1.494768
-Na	1	Cl	-1	6.52	1.69489	6.5	0.315458	2.748011	1.663894
-Mg	2	Cl	-1	5.897	1.78276	6.5	0.796023	2.393298	1.587302
-Al	3	Cl	-1	5.327	1.89795	6.5	1.367335	2.197469	1.547988
-P	5	Cl	-1	4	2.01093	7	2.935183	1.791686	1.510574
-K	1	Cl	-1	8.846	2.07673	6.5	0.201068	3.184081	1.801802
-Ca	2	Cl	-1	7.544	2.06262	6.5	0.53146	2.759777	1.683502
-Ga	3	Cl	-1	4.905	1.97794	6.5	0.959766	2.170468	1.730104
-Ge	4	Cl	-1	4.305	2.07619	6	1.521374	2.033413	1.639344
-Rb	1	Cl	-1	10.02	2.26585	6.5	0.155502	3.370857	1.883239
-Sr	2	Cl	-1	9.4	2.20197	6.5	0.408921	2.985294	1.745201
-In	3	Cl	-1	6.024	2.13474	6.5	0.695073	2.409564	1.824818
-Sn	4	Cl	-1	6.069	2.17643	6.5	1.106595	2.32334	1.70068
-Sb	5	Cl	-1	6	2.2232	6.5	1.572233	2.243372	1.623377
-Cs	1	Cl	-1	11.79	2.46037	6.5	0.119331	3.555351	2
-Ba	2	Cl	-1	10.32	2.41041	6.5	0.290875	3.143075	1.926782
-Tl	3	Cl	-1	5.22	2.22567	6	0.56302	2.389021	1.945525
-S	4	Cl	-1	3	2.05269	6.5	1.591239	1.791962	1.834862
-Ga	1	Cl	-1	4.905	2.3204	6	0.14014	2.871349	2.272727
-As	3	Cl	-1	3	2.06175	6	0.870752	1.951235	1.915709
-Se	4	Cl	-1	3	2.15849	6.5	1.304935	1.89237	1.834862
-In	1	Cl	-1	6.024	2.43863	6	0.105153	3.015535	2.421308
-Sb	3	Cl	-1	6	2.30831	6	0.544277	2.520874	2.016129
-Te	4	Cl	-1	3.396	2.30563	6.5	0.951857	2.09621	1.930502
-Tl	1	Cl	-1	8.03	2.36792	6	0.126355	3.237936	2.03666
-Pb	2	Cl	-1	7.541	2.34641	5.5	0.268937	2.83552	2.109705
-Bi	3	Cl	-1	6.058	2.34105	6	0.50612	2.565353	1.980198
-Sc	3	Cl	-1	6.255	2.1133	6.5	1.541393	2.474212	1.633987
-Ti	4	Cl	-1	6	2.12577	6	1.346432	2.244649	1.972387
-#Cr	6	Cl	-1	4	2.007	6.5	2.648568	2.185395	-1.577287
-Fe	3	Cl	-1	5.733	1.98266	6	1.322259	2.228926	1.858736
-Ni	2	Cl	-1	5.933	1.87666	5.5	0.825239	2.282632	2.10084
-Cu	2	Cl	-1	2.56	1.90175	5.5	0.964976	1.903186	2.12766
-Zn	2	Cl	-1	4.718	1.88195	6	1.012812	2.228172	1.919386
-Y	3	Cl	-1	7.285	2.28867	6.5	0.812042	2.616424	2.070393
-Zr	4	Cl	-1	6.765	2.18437	6.5	1.61247	2.41089	1.644737
-Nb	5	Cl	-1	6.044	2.20986	6.5	1.996217	2.234964	1.623377
-#Mo	6	Cl	-1	4.764	2.0888	6.5	2.320539	2.147333	-1.607717
-Pd	2	Cl	-1	4	1.99818	5	0.61099	2.157132	2.375297
-Ag	1	Cl	-1	4.438	1.98819	5	0.387504	2.497296	2.331002
-Cd	2	Cl	-1	6.176	2.0695	6	0.769487	2.533294	1.953125
-Lu	3	Cl	-1	6.83	2.284	6	0.617863	2.522817	2.309469
-Hf	4	Cl	-1	7.105	2.2444	6.5	0.924292	2.423017	2.070393
-Ta	5	Cl	-1	6.09	2.21442	6.5	1.749379	2.23829	1.655629
-W	6	Cl	-1	5.688	2.21497	7	2.141315	2.09029	1.620746
-Pt	2	Cl	-1	4	1.97699	5.5	0.65892	2.142168	2.192982
-Au	3	Cl	-1	4	2.14532	5.5	0.69387	2.123675	2.375297
-Hg	2	Cl	-1	6.966	2.17009	5.5	0.539918	2.602861	2.197802
-La	3	Cl	-1	9.83	2.43099	6	0.612367	2.860323	2.178649
-Pr	3	Cl	-1	9.067	2.48619	5.5	0.449895	2.767658	2.583979
-Ti	3	Cl	-1	6	2.13089	6	0.925547	2.317792	2.178649
-Fe	2	Cl	-1	5.743	2.00003	5	0.686296	2.334636	2.277904
-Rh	3	Cl	-1	6	2.03722	5	0.797203	2.211713	2.272727
-Pd	4	Cl	-1	5.333	2.12662	6	1.088684	2.133809	2.12766
-W	5	Cl	-1	6	2.24489	6	0.871662	2.172085	2.380952
-Hg	1	Cl	-1	4.786	2.17341	5.5	0.365096	2.721804	2.197802
-Ti	2	Cl	-1	6	2.03427	5.5	0.644954	2.372399	2.331002
-V	3	Cl	-1	6	2.06334	5.5	1.031449	2.274479	2.083333
-Cr	3	Cl	-1	6	2.0051	5.5	1.092685	2.228283	2.04499
-Co	2	Cl	-1	5.506	1.93137	5.5	0.795676	2.288535	2.136752
-Cu	1	Cl	-1	2.56	1.79822	5	0.462969	2.052044	2.487562
-Zr	2	Cl	-1	6.765	2.12072	6	0.670128	2.53539	2.09205
-Mo	4	Cl	-1	6	2.1283	6.5	1.489813	2.197852	1.792115
-Ir	3	Cl	-1	6	2.05823	5.5	0.612349	2.194093	2.487562
-Pt	4	Cl	-1	6	2.1411	6	0.851686	2.182212	2.272727
-V	2	Cl	-1	6	2.03267	5.5	0.679979	2.388641	2.262443
-Cr	2	Cl	-1	5.6	2.01499	5.5	0.685419	2.337625	2.277904
-Mn	4	Cl	-1	5.923	2.06541	6.5	1.457267	2.156547	1.934236
-Mo	3	Cl	-1	5.7	2.08941	6	0.996785	2.293329	1.996008
-Tc	4	Cl	-1	6	2.15861	6	1.046765	2.219262	2.12766
-Ru	3	Cl	-1	6	1.9952	5.5	0.981474	2.218867	2.04499
-W	3	Cl	-1	6	2.12237	5	0.672476	2.264711	2.336449
-Re	4	Cl	-1	6	2.18513	5.5	0.739216	2.204421	2.427184
-Mo	2	Cl	-1	5.5	2.05175	5.5	0.616601	2.345416	2.267574
-Os	4	Cl	-1	6	2.15572	6	0.779449	2.182969	2.375297
-Mn	2	Cl	-1	5.91	1.99681	6	0.821608	2.409777	2.04918
-Re	3	Cl	-1	6	2.15781	5.5	0.639211	2.294331	2.380952
-Eu	3	Cl	-1	7.743	2.31998	6	0.739494	2.644542	2.061856
-Gd	3	Cl	-1	8.052	2.27126	6	0.881597	2.679082	1.876173
-Tb	3	Cl	-1	7.958	2.29526	6	0.745002	2.635827	2.057613
-Dy	3	Cl	-1	7.828	2.2881	6	0.768339	2.629921	2.028398
-Er	3	Cl	-1	7.135	2.25982	6	0.830373	2.573621	1.972387
-Yb	2	Cl	-1	8	2.29464	5.5	0.419744	2.705315	2.444988
-Eu	2	Cl	-1	10.111	2.41447	5.5	0.416527	2.943683	2.352941
-Li	1	Br	-1	5.263	1.51288	7	0.44910 	2.58255 	1.481481
-#Be	2	Br	-1	4	1.6581	7	2.215989	1.122546	-1.430615
-#B	3	Br	-1	3.417	1.821	6.5	2.291796	1.675041	-1.410437
-Na	1	Br	-1	6.52	1.78228	7	0.292879	2.915883	1.560062
-Mg	2	Br	-1	5.897	1.89059	7	0.733669	2.551036	1.490313
-Al	3	Br	-1	5.327	2.04045	7	1.242373	2.36878	1.455604
-K	1	Br	-1	8.846	2.17206	7	0.188913	3.373219	1.680672
-#Ca	2	Br	-1	7.544	2.1686	7	1.165036	1.242057	-1.577287
-Ga	3	Br	-1	4.905	2.11352	6.5	0.887656	2.330935	1.615509
-Rb	1	Br	-1	10.02	2.34362	7	0.14833	3.55125	1.748252
-#Sr	2	Br	-1	9.4	2.3125	7	0.95906	1.265723	-1.628664
-In	3	Br	-1	6.024	2.28936	6.5	0.645222	2.596929	1.697793
-Cs	1	Br	-1	11.79	2.50818	7	0.115797	3.714691	1.848429
-#Ba	2	Br	-1	10.32	2.486	7	0.74336	1.399882	-1.680672
-Tl	3	Br	-1	5.22	2.35992	6	0.532392	2.550956	1.801802
-Se	4	Br	-1	3	2.32723	7	1.200099	2.05318	1.709402
-In	1	Br	-1	6.024	2.46665	6	0.106082	3.128138	2.202643
-Sb	3	Br	-1	6	2.38165	7	0.529405	2.630872	1.862197
-Te	4	Br	-1	3.396	2.46108	7	0.894624	2.249368	1.788909
-Tl	1	Br	-1	8.03	2.42772	6	0.102033	3.27736	2.096436
-Pb	2	Br	-1	7.541	2.4316	6	0.261373	2.982711	1.941748
-Bi	3	Br	-1	6.058	2.46708	7	0.480534	2.725316	1.834862
-#Cr	6	Br	-1	4	2.224	6.5	2.339341	2.421694	-1.48368
-Fe	3	Br	-1	5.733	2.13627	6.5	1.22157	2.411656	1.730104
-Ni	2	Br	-1	5.933	1.96729	6	0.791638	2.421615	1.937984
-Zn	2	Br	-1	4.718	1.98741	6	0.958104	2.373518	1.779359
-Y	3	Br	-1	7.285	2.40922	6.5	0.7734	2.778819	1.915709
-Zr	4	Br	-1	6.765	2.32815	7	1.481279	2.581699	1.54321
-#Mo	6	Br	-1	4.764	2.3037	6.5	2.064478	2.374953	-1.508296
-Pd	2	Br	-1	4	2.10183	5.5	0.599388	2.293259	2.164502
-Ag	1	Br	-1	4.438	2.03699	5.5	0.384726	2.614612	2.12766
-Cd	2	Br	-1	6.176	2.16913	6	0.733475	2.684989	1.808318
-Au	3	Br	-1	4	2.27911	5.5	0.673499	2.271943	2.169197
-Hg	2	Br	-1	6.966	2.25138	6	0.525569	2.740738	2.020202
-Fe	2	Br	-1	5.743	2.09517	5.5	0.666987	2.476774	2.087683
-Ti	2	Br	-1	6	2.15487	6	0.625835	2.541373	2.12766
-Cr	3	Br	-1	6	2.13165	6.5	1.037691	2.387051	1.886792
-Cu	1	Br	-1	2.56	1.8681	5.5	0.459534	2.164436	2.262443
-W	4	Br	-1	6	2.3517	6.5	0.67355	2.378816	2.277904
-V	2	Br	-1	6	2.10218	6	0.669272	2.509714	2.070393
-Cr	2	Br	-1	5.6	2.12678	6	0.66474	2.495533	2.083333
-Mo	3	Br	-1	5.7	2.19147	6	0.951252	2.426733	1.848429
-Mo	2	Br	-1	5.5	2.22218	5.5	0.418518	2.474296	2.493766
-W	2	Br	-1	6	1.95717	7	0.966423	2.546409	1.545595
-Os	4	Br	-1	6	2.30615	6	0.751339	2.351622	2.169197
-Mn	2	Br	-1	5.91	2.08701	6	0.787476	2.54896	1.893939
-Re	3	Br	-1	6	2.30419	5.5	0.524717	2.443614	2.369668
-Eu	2	Br	-1	10.111	2.50011	6	0.409845	3.10151	2.150538
-Li	1	I	-1	5.000	1.64829	7	0.44117	        2.78807 	1.360544
-#Be	2	I	-1	4	1.8008	7	2.134019	1.232513	-1.315789
-#B	3	I	-1	3.417	2.007	7	2.173632	1.863156	-1.298701
-Na	1	I	-1	6.52	1.94353	7	0.285612	3.198502	1.426534
-#Mg	2	I	-1	5.897	2.045	7	1.655681	1.199982	-1.367989
-Al	3	I	-1	5.327	2.24648	7	1.187824	2.619974	1.338688
-P	5	I	-1	4	2.49792	7.5	2.382629	2.27117	1.310616
-K	1	I	-1	8.846	2.2888	7	0.190106	3.633321	1.526718
-#Ca	2	I	-1	7.544	2.3242	7	1.170657	1.328579	-1.438849
-#Ga	3	I	-1	4.905	2.314	7	1.170186	1.902933	-1.472754
-Rb	1	I	-1	10.02	2.46445	7	0.150421	3.823732	1.582278
-#Sr	2	I	-1	9.4	2.3242	7	1.189417	1.169575	-1.438849
-In	3	I	-1	6.024	2.47773	7	0.674268	2.850379	1.49925
-Cs	1	I	-1	11.79	2.71194	8	0.116459	4.07706	1.663894
-#Ba	2	I	-1	10.32	2.6495	7.5	0.763038	1.478218	-1.526718
-Ga	1	I	-1	4.905	2.38769	7	0.150745	3.125864	1.848429
-In	1	I	-1	6.024	2.50769	7	0.115503	3.293778	1.945525
-Sb	3	I	-1	6	2.59905	7.5	0.531155	2.898754	1.675042
-Te	4	I	-1	3.396	2.67663	7.5	0.895233	2.465289	1.615509
-Tl	1	I	-1	8.03	2.48689	7	0.109014	3.477263	1.862197
-Pb	2	I	-1	7.541	2.5688	7	0.270625	3.211959	1.73913
-Bi	3	I	-1	6.058	2.63989	7.5	0.488978	2.951989	1.652893
-#Cr	6	I	-1	4	2.5373	7	2.176374	2.768722	-1.360544
-Fe	3	I	-1	5.733	2.37658	6	0.822293	2.623615	1.912046
-Zn	2	I	-1	4.718	2.15151	6.5	0.959066	2.597824	1.607717
-#Mo	6	I	-1	4.764	2.6191	7	1.922048	2.713286	-1.383126
-Ag	1	I	-1	4.438	2.08036	6	0.414392	2.760885	1.886792
-Cd	2	I	-1	6.176	2.3244	7	0.741701	2.918199	1.631321
-Hf	4	I	-1	7.105	2.57677	7	0.895483	2.832144	1.712329
-Hg	2	I	-1	6.966	2.38163	6	0.547753	2.956874	1.801802
-Fe	2	I	-1	5.743	2.25785	6	0.692512	2.711676	1.851852
-Zr	3	I	-1	6.765	2.56625	6	0.562056	2.796227	2.118644
-Co	2	I	-1	5.506	2.19837	6	0.780849	2.670145	1.757469
-Cu	1	I	-1	2.56	1.93067	6	0.501948	2.295302	1.988072
-Zr	2	I	-1	6.765	2.49296	5.5	0.36402	2.844654	2.358491
-Cr	2	I	-1	5.6	2.28404	6.5	0.689638	2.722975	1.851852
-Mo	2	I	-1	5.5	2.35705	6	0.456968	2.678791	2.169197
-Mn	2	I	-1	5.91	2.26045	6.5	0.796403	2.795756	1.70068
-Eu	2	I	-1	10.111	2.66292	6.5	0.429764	3.372258	1.904762
-Li	1	N	-3	5.021	1.1543	6	2.054953	2.132557	1.569859
-Mg	2	N	-3	5.897	1.63729	6	2.874771	2.215919	1.663894
-Sr	2	N	-3	9.4	2.09477	6.5	1.428465	2.830165	1.838235
-Cr	6	N	-3	4	1.96859	6.5	6.823816	1.638522	1.652893
-Nb	5	N	-3	6.044	2.0288	5	2.833875	2.027799	2.083333
-Eu	3	N	-3	7.743	2.1627	6	1.484427	2.459643	2.197802
-Gd	3	N	-3	8.052	2.09519	6.5	1.809718	2.475474	1.984127
-Eu	2	N	-3	10.111	2.1874	6	0.974842	2.731273	2.325581
+cation	cation_valence	anion	anion_valence	Nc	R0	Rcutoff	D0	Rmin	alpha
+Li	1	O	-2	5.021	1.17096	6	0.98816	1.940013	1.937984
+Be	2	O	-2	4	1.20903	5.5	2.768816	1.522169	1.848429
+B	3	O	-2	3.417	1.35761	4.5	2.389237	1.340034	2.597403
+C	4	O	-2	3	1.39826	5	4.791867	1.200889	2.237136
+N	5	O	-2	3	1.46267	5	6.276775	1.161424	2.222222
+Na	1	O	-2	6.52	1.56225	6	0.575227	2.374335	2.293578
+Mg	2	O	-2	5.897	1.48398	5.5	1.575539	1.956265	1.953125
+Al	3	O	-2	5.327	1.59901	5	1.803461	1.758058	2.358491
+Si	4	O	-2	4.1	1.60817	5	2.857198	1.535939	2.314815
+P	5	O	-2	4	1.62038	5	3.896352	1.44066	2.28833
+S	6	O	-2	4	1.6422	5	4.96726	1.381015	2.267574
+Cl	7	O	-2	4	1.67946	5	5.991005	1.348009	2.257336
+K	1	O	-2	8.846	1.94117	6	0.34985	2.766359	2.293578
+Ca	2	O	-2	7.544	1.79519	5.5	0.994291	2.32032	2.10084
+Ga	3	O	-2	4.905	1.71606	5	1.184556	1.79391	2.680965
+Ge	4	O	-2	4.305	1.73939	5	1.913747	1.66872	2.525253
+As	5	O	-2	4.029	1.76689	5	2.719344	1.581273	2.43309
+Se	6	O	-2	4	1.79866	5.5	3.448655	1.532871	2.403846
+Br	7	O	-2	4	1.83658	5.5	4.243387	1.502739	2.364066
+Rb	1	O	-2	10.02	2.08597	6.5	0.268127	2.896827	2.421308
+Sr	2	O	-2	9.4	1.95311	5.5	0.743506	2.535891	2.197802
+In	3	O	-2	6.024	1.90305	5	0.840758	2.024707	2.832861
+Sn	4	O	-2	6.069	1.89019	5	1.352679	1.934221	2.638522
+Sb	5	O	-2	6	1.89768	5.5	1.955227	1.863182	2.5
+Te	6	O	-2	6	1.91343	5.5	2.564057	1.808758	2.427184
+I	7	O	-2	5.8	1.92274	5.5	3.214242	1.741045	2.386635
+Cs	1	O	-2	11.79	2.25899	6.5	0.233071	3.131213	2.386635
+Ba	2	O	-2	10.32	2.15998	6	0.579936	2.737692	2.28833
+Tl	3	O	-2	5.22	2.06297	5	0.676365	2.106422	2.95858
+Pb	4	O	-2	5.74	2.03293	5	1.027186	2.028568	2.824859
+Bi	5	O	-2	6	2.04498	5	1.4405	1.985987	2.695418
+C	2	O	-2	1	1.41368	5	2.405528	1.030976	2.409639
+N	3	O	-2	2	1.40795	5	3.81089	1.137584	2.232143
+P	3	O	-2	3	1.51555	4.5	2.020615	1.410511	2.487562
+S	4	O	-2	3	1.64282	5.5	3.036723	1.411879	2.34192
+As	3	O	-2	3	1.76706	5	1.514929	1.645543	2.475248
+Se	4	O	-2	3	1.80095	5.5	2.380823	1.559575	2.34192
+Sn	2	O	-2	3.325	1.87499	5.5	0.972609	1.964197	2.183406
+Sb	3	O	-2	6	1.92036	5	1.177857	2.075258	2.364066
+Te	4	O	-2	3.396	1.9529	5.5	1.671694	1.752082	2.493766
+I	5	O	-2	3.1	1.97775	6	2.489472	1.644209	2.358491
+Tl	1	O	-2	8.03	1.91752	6	0.349987	2.77086	2.070393
+Pb	2	O	-2	7.541	2.01825	5.5	0.638333	2.441914	2.309469
+Bi	3	O	-2	6.058	2.03677	5.5	0.979037	2.183207	2.415459
+Te	2	O	-2	2	1.39168	6.5	2.626094	1.298928	1.633987
+Sc	3	O	-2	6.255	1.7322	5.5	2.156103	1.996147	2.024291
+Ti	4	O	-2	6	1.72394	5.5	2.813331	1.83144	1.988072
+V	5	O	-2	4.166	1.79445	5.5	3.695335	1.602577	1.960784
+Cr	6	O	-2	4	1.82471	5.5	3.687511	1.532511	2.10084
+Mn	7	O	-2	4	1.87362	6.5	4.916305	1.481714	1.923077
+Fe	3	O	-2	5.733	1.7084	5	1.66681	1.866468	2.380952
+Co	3	O	-2	6	1.59234	5.5	1.870235	1.776198	2.304147
+Ni	2	O	-2	5.933	1.5592	5.5	1.468407	1.924524	2.257336
+Cu	2	O	-2	2.56	1.57422	5	1.853408	1.566333	2.227171
+Zn	2	O	-2	4.718	1.65344	5	1.24031	1.885568	2.48139
+Y	3	O	-2	7.285	1.90384	5.5	1.627011	2.215228	2.09205
+Zr	4	O	-2	6.765	1.84505	5.5	2.191032	1.996025	2.040816
+Nb	5	O	-2	6.044	1.86588	5.5	2.723261	1.854586	2.008032
+Mo	6	O	-2	4.764	1.90934	5	1.991498	1.712544	2.557545
+Tc	7	O	-2	4	1.97036	6	4.041444	1.575183	1.945525
+Ru	6	O	-2	4.5	1.92579	5.5	2.421093	1.664311	2.352941
+Rh	4	O	-2	6	1.77675	5.5	1.627252	1.817932	2.48139
+Pd	2	O	-2	4	1.62359	5.5	1.739103	1.836711	2.008032
+Ag	1	O	-2	4.438	1.78239	5	0.635187	2.225785	2.538071
+Cd	2	O	-2	6.176	1.83926	5.5	0.983461	2.169398	2.457002
+Lu	3	O	-2	6.83	1.91728	5.5	1.194883	2.136	2.375297
+Hf	4	O	-2	7.105	1.83361	6	1.89992	1.999643	2.09205
+Ta	5	O	-2	6.09	1.86816	5.5	2.366685	1.85532	2.057613
+W	6	O	-2	5.688	1.90641	5	1.842666	1.777132	2.493766
+Re	7	O	-2	4.098	1.97792	6	3.555929	1.596339	1.968504
+Os	8	O	-2	5.333	1.97728	6	3.710191	1.661463	1.953125
+Ir	5	O	-2	6	1.89791	6	2.324762	1.83476	2.087683
+Pt	2	O	-2	4	1.51205	5.5	2.149986	1.801793	1.74216
+Au	3	O	-2	4	1.81761	5.5	1.969672	1.813123	2.008032
+Hg	2	O	-2	6.966	1.81276	5.5	1.128521	2.252751	2.150538
+La	3	O	-2	9.83	2.06392	5.5	1.185874	2.469886	2.217295
+Ce	4	O	-2	7.867	2.02821	5.5	1.484118	2.198725	2.257336
+Pr	3	O	-2	9.067	2.03652	5.5	1.170407	2.371126	2.277904
+Nd	3	O	-2	8.647	2.02425	5.5	1.132045	2.330162	2.336449
+Ti	3	O	-2	6	1.69766	5.5	1.978506	1.886194	2.173913
+V	4	O	-2	5.738	1.74932	5	2.080473	1.776375	2.347418
+Cr	4	O	-2	5.429	1.76095	5.5	1.933285	1.76209	2.444988
+Mn	6	O	-2	4	1.82018	5.5	2.822364	1.529314	2.403846
+Fe	2	O	-2	5.743	1.57911	5.5	1.692689	1.960053	2.083333
+Co	4	O	-2	4	1.79444	5.5	2.358037	1.679593	2.267574
+Ni	4	O	-2	6	1.72159	5	1.864513	1.765079	2.487562
+Cu	3	O	-2	4	1.70964	5	1.882423	1.708232	2.34192
+Nb	4	O	-2	6	1.78543	6	2.709602	1.859895	1.901141
+Mo	5	O	-2	5.98	1.8476	5.5	2.648016	1.786697	2.074689
+Ru	5	O	-2	6	1.87442	5.5	2.132078	1.815714	2.293578
+Rh	3	O	-2	6	1.67013	5.5	1.928259	1.869147	2.09205
+Pd	4	O	-2	5.333	1.805	5.5	2.042177	1.798133	2.227171
+Ag	3	O	-2	6.25	1.84687	5.5	1.52826	2.0348	2.252252
+Ta	4	O	-2	5.5	1.75632	6	2.756548	1.798256	1.831502
+W	5	O	-2	6	1.81975	6	2.615701	1.762615	2.008032
+Re	6	O	-2	5.5	1.91007	6	2.950986	1.711469	2.008032
+Os	7	O	-2	6	1.95775	5.5	2.919483	1.728686	2.087683
+Ir	4	O	-2	6	1.83233	5.5	1.686674	1.874017	2.293578
+Hg	1	O	-2	4.786	1.8128	5.5	0.739306	2.431553	2.150538
+V	3	O	-2	6	1.67799	5.5	1.82936	1.857967	2.277904
+Cr	3	O	-2	6	1.66198	5.5	1.773346	1.838872	2.325581
+Mn	5	O	-2	4	1.78879	5.5	2.464555	1.575774	2.421308
+Fe	4	O	-2	6	1.76559	5.5	1.872848	1.827859	2.439024
+Co	2	O	-2	5.506	1.59773	5.5	1.514761	1.933621	2.217295
+Ni	3	O	-2	6	1.64888	5.5	1.661905	1.818873	2.415459
+Cu	1	O	-2	2.56	1.5873	5	0.664171	1.782692	2.932551
+Nb	3	O	-2	6	1.74581	6	2.028483	1.951898	1.996008
+Mo	4	O	-2	6	1.7239	6.5	3.108069	1.850992	1.779359
+Ru	4	O	-2	6	1.79363	5.5	1.995133	1.840532	2.227171
+Ag	2	O	-2	5	1.72209	5.5	1.583396	2.041706	1.996008
+W	4	O	-2	6	1.74558	6	2.471141	1.819454	1.923077
+Re	5	O	-2	6	1.82664	6	2.41099	1.769141	2.087683
+Os	6	O	-2	6	1.93192	5.5	2.448709	1.782799	2.159827
+Pt	4	O	-2	6	1.82198	5.5	2.038254	1.871736	2.087683
+Au	1	O	-2	2	1.71819	5.5	0.853044	1.895429	2.267574
+V	2	O	-2	6	1.59976	5.5	1.640237	1.997526	2.096436
+Cr	2	O	-2	5.6	1.59356	5.5	1.691613	1.961299	2.083333
+Mn	4	O	-2	5.923	1.73272	5	1.858861	1.770446	2.487562
+Co	1	O	-2	2	1.29501	5.5	2.393481	1.640592	1.610306
+Mo	3	O	-2	5.7	1.78933	5.5	1.428262	1.929735	2.392344
+Ru	3	O	-2	6	1.72066	5.5	1.540613	1.8932	2.325581
+Re	4	O	-2	6	1.78237	6	2.316639	1.844971	1.972387
+Pt	3	O	-2	5	1.66559	5.5	2.359527	1.819377	1.831502
+Cr	5	O	-2	4	1.76781	5.5	2.365511	1.555463	2.487562
+Mn	3	O	-2	5.862	1.68993	5.5	1.812832	1.857862	2.28833
+Os	4	O	-2	6	1.75302	6	2.27524	1.812439	2.008032
+Mn	2	O	-2	5.91	1.62758	5.5	1.641434	2.029688	2.079002
+Ce	3	O	-2	9.147	2.03118	5.5	1.220483	2.37861	2.227171
+Sm	3	O	-2	8.119	2.01168	5.5	1.176217	2.295359	2.309469
+Eu	3	O	-2	7.743	2.00469	5.5	1.195447	2.268881	2.304147
+Gd	3	O	-2	8.052	1.99654	5.5	1.091613	2.271904	2.409639
+Tb	3	O	-2	7.958	1.95675	5.5	1.20764	2.235634	2.309469
+Dy	3	O	-2	7.828	1.96029	5.5	1.173498	2.226892	2.347418
+Ho	3	O	-2	7.5	1.97099	5.5	1.121573	2.211215	2.409639
+Er	3	O	-2	7.135	1.95608	5.5	1.123941	2.174771	2.427184
+Tm	3	O	-2	6.912	1.94901	5.5	1.181379	2.160417	2.375297
+Yb	3	O	-2	6.875	1.92872	5.5	1.219894	2.142197	2.347418
+Yb	2	O	-2	8	1.63254	5.5	1.384137	2.209419	1.960784
+Eu	2	O	-2	10.111	1.89158	6	1.130318	2.538459	2.024291
+Tb	4	O	-2	6	1.96244	6	1.701319	2.385063	2.024291
+Th	4	O	-2	8.941	2.04983	6	1.573737	2.310462	2.057613
+U	6	O	-2	6.987	2.02317	6	2.627524	1.992868	1.897533
+Cl	5	O	-2	3	1.69552	5.5	4.290893	1.356529	2.247191
+Cl	3	O	-2	2	1.72265	5.5	3.071187	1.384411	2.03666
+Li	1	S	-2	4.604	1.46652	6	1.04027  	2.40971 	1.531394
+#Be	2	S	-2	4	1.5784	6.5	5.102614	1.056091	-1.477105
+B	3	S	-2	3.417	1.78195	6	3.21881	1.798962	1.745201
+C	4	S	-2	3	1.84354	6	4.870252	1.618649	1.727116
+Na	1	S	-2	6.52	1.83088	6.5	0.630673	2.916205	1.615509
+Mg	2	S	-2	5.897	1.82372	6.5	1.645364	2.457529	1.540832
+Al	3	S	-2	5.327	2.05965	6	1.891546	2.302878	1.818182
+Si	4	S	-2	4.1	2.09975	6.5	2.948361	2.042192	1.785714
+P	5	S	-2	4	2.14917	6	3.939695	1.951558	1.766784
+S	6	S	-2	4	2.2	5.5	4.950597	1.896737	1.751313
+K	1	S	-2	8.846	2.16803	6.5	0.41168	3.315285	1.745201
+Ca	2	S	-2	7.544	2.11148	7	1.098221	2.835405	1.633987
+Ga	3	S	-2	4.905	2.12458	6	1.282374	2.268677	2.070393
+Ge	4	S	-2	4.305	2.19183	6	2.050539	2.142348	1.945525
+As	5	S	-2	4.029	2.27986	6.5	2.850033	2.079575	1.872659
+Rb	1	S	-2	10.02	2.30817	6.5	0.325038	3.460253	1.818182
+Sr	2	S	-2	9.4	2.26765	7	0.842963	3.081154	1.692047
+In	3	S	-2	6.024	2.30797	6	0.92204	2.515464	2.192982
+Sn	4	S	-2	6.069	2.36256	6	1.459465	2.466684	2.03252
+Sb	5	S	-2	6	2.44254	6	2.058532	2.441945	1.923077
+Cs	1	S	-2	11.79	2.52283	6.5	0.249303	3.667187	1.926782
+Ba	2	S	-2	10.32	2.44239	7	0.682017	3.267913	1.745201
+P	3	S	-2	3	1.96089	6	2.224943	1.859402	1.865672
+As	3	S	-2	3	2.20841	6	1.735537	2.095302	1.851852
+Sn	2	S	-2	3.325	2.32497	6	0.701776	2.431194	2.087683
+Sb	3	S	-2	6	2.36947	6	1.138983	2.597379	1.941748
+Tl	1	S	-2	8.03	2.3826	6	0.2208	3.182358	2.197802
+Pb	2	S	-2	7.541	2.38758	6	0.567913	2.905146	2.028398
+Bi	3	S	-2	6.058	2.41824	6.5	1.048372	2.656656	1.912046
+Sc	3	S	-2	6.255	2.0945	7	2.316425	2.475159	1.584786
+Ti	4	S	-2	6	2.17452	7	2.897523	2.350525	1.5625
+V	5	S	-2	4.166	2.29252	7	3.726229	2.088459	1.545595
+#Cr	6	S	-2	4	2.103	6.5	3.780483	2.289947	-1.533742
+Ni	2	S	-2	5.933	1.85695	5.5	1.253997	2.288097	2.024291
+Cu	2	S	-2	2.56	1.94997	6	1.430321	1.957596	2.04918
+Zn	2	S	-2	4.718	1.94373	6	1.485755	2.307582	1.851852
+Y	3	S	-2	7.285	2.25923	7	1.797063	2.710781	1.626016
+Zr	4	S	-2	6.765	2.26265	7	2.330585	2.500694	1.597444
+#Mo	6	S	-2	4.764	2.187	6.5	3.324576	2.251139	-1.560062
+Pd	2	S	-2	4	2.02559	5.5	0.921219	2.200028	2.277904
+Ag	1	S	-2	4.438	2.11006	5	0.392994	2.520847	2.739726
+Cd	2	S	-2	6.176	2.12789	5.5	1.13392	2.614981	1.883239
+Lu	3	S	-2	6.83	2.28119	7	1.388246	2.627609	1.795332
+Hf	4	S	-2	7.105	2.2355	7	2.057539	2.495677	1.626016
+Ta	5	S	-2	6.09	2.2786	6.5	2.543639	2.308695	1.607717
+Pt	2	S	-2	4	2.0245	5.5	0.845436	2.178404	2.283105
+Hg	2	S	-2	6.966	2.20501	5.5	0.806433	2.66333	2.114165
+La	3	S	-2	9.83	2.4033	6.5	1.358302	2.992782	1.70068
+Pr	3	S	-2	9.067	2.46496	6	1.017448	2.877435	2.004008
+Nd	3	S	-2	8.647	2.44624	6	1.072575	2.851212	1.960784
+Ti	3	S	-2	6	2.11813	6	1.415711	2.32404	2.09205
+V	4	S	-2	5.738	2.1676	6.5	1.951626	2.233445	1.953125
+Fe	2	S	-2	5.743	2.01111	5.5	1.036628	2.368789	2.188184
+Nb	4	S	-2	6	2.28012	5.5	1.101045	2.2928	2.427184
+Ta	4	S	-2	5.5	2.28935	5.5	1.010309	2.258914	2.439024
+V	3	S	-2	6	2.02622	6.5	1.588277	2.25755	2.004008
+Cr	3	S	-2	6	2.04397	5.5	1.627769	2.282954	1.968504
+Co	2	S	-2	5.506	1.99705	5.5	1.174488	2.374249	2.053388
+Ni	3	S	-2	6	1.95763	5.5	1.777739	2.215633	1.912046
+Cu	1	S	-2	2.56	1.80744	5	0.704448	2.08186	2.380952
+W	4	S	-2	6	2.22672	6	1.050809	2.246646	2.398082
+Pt	4	S	-2	6	2.19999	6	1.265783	2.249872	2.183406
+Au	1	S	-2	2	2.06404	4.5	0.368405	2.155176	2.923977
+V	2	S	-2	6	1.89815	6	1.092053	2.288101	2.169197
+Cr	2	S	-2	5.6	1.9093	5.5	1.089919	2.262838	2.183406
+Mn	4	S	-2	5.923	2.30057	6	1.997166	2.391923	1.865672
+Mo	3	S	-2	5.7	2.06172	6	1.519179	2.283669	1.926782
+Re	4	S	-2	6	2.268	6	1.098995	2.294802	2.320186
+Mo	2	S	-2	5.5	2.07169	5.5	0.797065	2.349596	2.369668
+Mn	2	S	-2	5.91	2.15468	5.5	0.783125	2.474786	2.463054
+Re	3	S	-2	6	2.2071	6	0.810667	2.332185	2.493766
+Ce	3	S	-2	9.147	2.50404	6	0.968018	2.904365	2.04499
+Sm	3	S	-2	8.119	2.4146	6	1.077495	2.782816	1.980198
+Eu	3	S	-2	7.743	2.39179	6	1.087691	2.734937	1.988072
+Gd	3	S	-2	8.052	2.37028	6	1.280701	2.797353	1.811594
+Tb	3	S	-2	7.958	2.36384	6	1.100521	2.724591	1.980198
+Dy	3	S	-2	7.828	2.34124	6	1.13993	2.703826	1.953125
+Ho	3	S	-2	7.5	2.33798	6	1.190448	2.691208	1.915709
+Er	3	S	-2	7.135	2.32366	6	1.220568	2.655055	1.904762
+Tm	3	S	-2	6.912	2.3107	6	1.196692	2.615977	1.937984
+Yb	3	S	-2	6.875	2.31245	6	1.176666	2.609189	1.956947
+Yb	2	S	-2	8	2.40079	6	0.617429	2.834914	2.34192
+Eu	2	S	-2	10.111	2.47173	6	0.621323	3.032226	2.257336
+Th	4	S	-2	8.941	2.45709	7	1.499684	2.809767	1.727116
+Li	1	Se	-2	5.118	1.62021	7	0.88750 	2.68386 	1.461988
+#Be	2	Se	-2	4	1.7043	7	4.388588	1.163025	-1.412429
+#B	3	Se	-2	3.417	1.9187	6	3.152102	1.785319	-1.647446
+Na	1	Se	-2	6.52	1.8988	7	0.576407	3.046979	1.538462
+#Mg	2	Se	-2	5.897	1.7043	7	4.725019	0.881992	-1.412429
+Al	3	Se	-2	5.327	2.17392	6.5	1.73113	2.440109	1.718213
+Si	4	Se	-2	4.1	2.23551	5.5	2.133055	2.181429	1.890359
+P	5	Se	-2	4	2.43695	7	3.352569	2.231858	1.666667
+K	1	Se	-2	8.846	2.29712	7	0.373639	3.51499	1.655629
+Ca	2	Se	-2	7.544	2.20285	7	1.001348	2.972826	1.55521
+Ga	3	Se	-2	4.905	2.24723	6.5	1.179547	2.40959	1.949318
+Ge	4	Se	-2	4.305	2.33264	6	1.868512	2.289073	1.834862
+Rb	1	Se	-2	10.02	2.40364	7	0.298431	3.629609	1.724138
+Sr	2	Se	-2	9.4	2.36718	7	0.770499	3.2336	1.607717
+In	3	Se	-2	6.024	2.43051	6	0.85029	2.661292	2.066116
+Sn	4	Se	-2	6.069	2.50725	6	1.335624	2.62763	1.915709
+Sb	5	Se	-2	6	2.58978	7	1.880426	2.599348	1.814882
+Cs	1	Se	-2	11.79	2.64858	7	0.229573	3.87313	1.818182
+Ba	2	Se	-2	10.32	2.51975	7	0.712287	3.476334	1.540832
+As	3	Se	-2	3	2.34035	6.5	1.579204	2.229757	1.751313
+Sb	3	Se	-2	6	2.47586	6.5	1.055133	2.729272	1.831502
+Tl	1	Se	-2	8.03	2.39935	6.5	0.228618	3.317982	1.968504
+Pb	2	Se	-2	7.541	2.46755	6.5	0.532474	3.031456	1.908397
+Bi	3	Se	-2	6.058	2.54545	7	0.963506	2.808944	1.805054
+#Cr	6	Se	-2	4	2.3	7	3.289049	2.501378	-1.464129
+Ni	2	Se	-2	5.933	1.89863	6	1.184866	2.368628	1.904762
+Cu	2	Se	-2	2.56	2.02888	6	1.339462	2.047631	1.926782
+Zn	2	Se	-2	4.718	2.00075	6	1.385461	2.396213	1.751313
+#Mo	6	Se	-2	4.764	2.3824	6.5	2.900851	2.455649	-1.488095
+Pd	2	Se	-2	4	2.13063	6	0.867507	2.328957	2.123142
+Ag	1	Se	-2	4.438	2.17409	5	0.364436	2.619255	2.597403
+Cd	2	Se	-2	6.176	2.16209	6.5	1.065618	2.689779	1.782531
+Hf	4	Se	-2	7.105	2.37893	7.5	1.839029	2.659792	1.550388
+Ta	5	Se	-2	6.09	2.51263	7	2.205338	2.549483	1.529052
+Pt	2	Se	-2	4	2.16525	6	0.599859	2.295839	2.457002
+Hg	2	Se	-2	6.966	2.25179	6	0.766574	2.754918	1.984127
+Pr	3	Se	-2	9.067	2.52676	7	0.956529	2.978932	1.890359
+Pd	4	Se	-2	5.333	2.31115	6.5	1.490694	2.336285	1.923077
+Ta	4	Se	-2	5.5	2.36128	6	0.895197	2.338963	2.369668
+V	3	Se	-2	6	2.13686	6.5	1.464549	2.391889	1.886792
+Cr	3	Se	-2	6	2.14649	6	1.503457	2.409792	1.855288
+Co	2	Se	-2	5.506	2.10951	6	1.084223	2.519929	1.930502
+Cu	1	Se	-2	2.56	1.89561	5.5	0.665431	2.200809	2.217295
+Pt	4	Se	-2	6	2.30943	6	1.184141	2.374275	2.04499
+Au	1	Se	-2	2	2.17613	4	0.309936	2.270736	2.890173
+Mn	2	Se	-2	5.91	2.24751	5.5	0.727927	2.598448	2.320186
+Ce	3	Se	-2	9.147	2.52663	7	0.92697	2.970218	1.923077
+Er	3	Se	-2	7.135	2.4342	7	1.125706	2.796224	1.798561
+Yb	3	Se	-2	6.875	2.42113	7	1.088819	2.7472	1.845018
+Yb	2	Se	-2	8	2.62618	7	0.562768	3.098868	2.183406
+Th	4	Se	-2	8.941	2.5485	7.5	1.385614	2.932808	1.636661
+Li	1	Te	-2	4.333	1.71028	7	0.88544 	2.73313 	1.371742
+#Be	2	Te	-2	4	1.8497	7	4.022722	1.283697	-1.328021
+#B	3	Te	-2	3.417	2.0982	6.5	3.018917	1.965185	-1.517451
+Na	1	Te	-2	6.52	2.03011	7	0.549276	3.269608	1.438849
+#Mg	2	Te	-2	5.897	1.9497	7	2.962016	1.160853	-1.470588
+Al	3	Te	-2	5.327	2.38658	7	1.657011	2.688729	1.582278
+K	1	Te	-2	8.846	2.41802	7	0.362353	3.742871	1.540832
+#Ca	2	Te	-2	7.544	2.3886	7	2.188266	1.397063	-1.451379
+Ga	3	Te	-2	4.905	2.44491	7	1.141133	2.63573	1.792115
+Ge	4	Te	-2	4.305	2.57461	7	1.782504	2.540892	1.686341
+Rb	1	Te	-2	10.02	2.43463	7.5	0.298622	3.779363	1.597444
+#Sr	2	Te	-2	9.4	2.5405	7	1.812178	1.418321	-1.497006
+In	3	Te	-2	6.024	2.62278	6.5	0.850959	2.89526	1.872659
+Sn	4	Te	-2	6.069	2.73112	7	1.291437	2.877902	1.760563
+Cs	1	Te	-2	11.79	2.78226	7.5	0.225509	4.127357	1.680672
+Ba	2	Te	-2	10.32	2.68807	7	0.606266	3.65307	1.540832
+Ge	2	Te	-2	4.305	2.26937	7	0.842876	2.614722	1.709402
+As	3	Te	-2	3	2.48812	7	1.536863	2.385037	1.623377
+Sb	3	Te	-2	6	2.73139	7	0.9996	3.018997	1.692047
+Tl	1	Te	-2	8.03	2.50518	6	0.213006	3.480158	1.883239
+Bi	3	Te	-2	6.058	2.82304	7	0.906776	3.120878	1.669449
+Ti	4	Te	-2	6	2.41793	7.5	2.501975	2.639068	1.396648
+Cr	6	Te	-2	4	2.609	8	3.737637	2.242906	1.371742
+Ni	2	Te	-2	5.933	2.11175	6.5	1.127862	2.632744	1.751313
+Zn	2	Te	-2	4.718	2.15126	7	1.333912	2.590758	1.623377
+#Mo	6	Te	-2	4.764	2.66	6.5	2.637957	2.749595	-1.3947
+Ag	1	Te	-2	4.438	2.34487	5	0.357046	2.845751	2.380952
+Cd	2	Te	-2	6.176	2.36683	7	1.017319	2.950242	1.647446
+Ta	5	Te	-2	6.09	2.71824	7	2.072226	2.772261	1.430615
+Hg	2	Te	-2	6.966	2.37917	7	0.760988	2.945194	1.821494
+Cr	3	Te	-2	6	2.30242	6.5	1.461856	2.602311	1.712329
+Cu	1	Te	-2	2.56	1.89529	6	0.70548	2.254788	2.012072
+Cr	2	Te	-2	5.6	2.18257	6.5	0.991672	2.618827	1.872659
+Nb	2	Te	-2	6	2.39087	6	0.598344	2.732389	2.232143
+Ta	2	Te	-2	6	2.20689	6	0.966348	2.705968	1.686341
+Mn	2	Te	-2	5.91	2.43113	6	0.71114	2.829003	2.12766
+Sm	3	Te	-2	8.119	2.71979	7	0.968805	3.173281	1.72117
+Li	1	F	-1	5.289	1.08674	6	0.49611 	1.87265 	1.968504
+Be	2	F	-1	4	1.14986	5.5	1.39717	1.4585	1.879699
+B	3	F	-1	3.417	1.19909	5	2.625262	1.208508	1.845018
+C	4	F	-1	3	1.37249	6	3.759427	1.146081	1.828154
+N	5	F	-1	3	1.40717	6	5.156374	1.055975	1.818182
+Na	1	F	-1	6.52	1.42885	5.5	0.295862	2.232158	2.109705
+Mg	2	F	-1	5.897	1.40956	5.5	0.796133	1.875696	1.984127
+Al	3	F	-1	5.327	1.4197	5.5	1.447303	1.64117	1.926782
+Si	4	F	-1	4.1	1.45654	5.5	2.362172	1.39289	1.890359
+P	5	F	-1	4	1.4761	7	3.28597	1.280179	1.869159
+S	6	F	-1	4	1.55	5	2.655352	1.291705	2.267574
+K	1	F	-1	8.846	1.83331	5.5	0.176234	2.645968	2.336449
+Ca	2	F	-1	7.544	1.71038	5.5	0.498644	2.226693	2.141328
+Ga	3	F	-1	4.905	1.56039	5.5	0.922174	1.684414	2.217295
+Ge	4	F	-1	4.305	1.57864	5.5	1.567311	1.521889	2.066116
+As	5	F	-1	4.029	1.60379	6	2.291271	1.405455	1.988072
+Rb	1	F	-1	10.02	1.99137	5.5	0.133404	2.785647	2.475248
+Sr	2	F	-1	9.4	1.86817	5.5	0.371198	2.440209	2.242152
+In	3	F	-1	6.024	1.75728	5.5	0.626012	1.933906	2.375297
+Sn	4	F	-1	6.069	1.75558	5.5	1.051935	1.839948	2.169197
+Sb	5	F	-1	6	1.76603	6	1.552674	1.753234	2.04499
+Xe	6	F	-1	4	1.86157	6	1.621152	1.565362	2.320186
+Cs	1	F	-1	11.79	2.15318	6	0.12472	3.052764	2.336449
+Ba	2	F	-1	10.32	2.06475	6	0.289369	2.631527	2.336449
+Tl	3	F	-1	5.22	1.857	5.5	0.345633	1.905526	3.076923
+Pb	4	F	-1	5.74	1.93428	5.5	0.76278	1.959449	2.358491
+Bi	5	F	-1	6	1.86984	5.5	1.137508	1.833638	2.232143
+As	3	F	-1	3	1.683	5	0.804158	1.565379	2.463054
+Sb	3	F	-1	6	1.83448	5.5	0.634722	1.999054	2.320186
+Xe	4	F	-1	4	1.85567	6.5	1.488549	1.712146	1.890359
+Tl	1	F	-1	8.03	1.82737	6	0.185412	2.702515	2.03666
+Pb	2	F	-1	7.541	1.90916	6	0.360632	2.365394	2.207506
+Bi	3	F	-1	6.058	1.93046	5.5	0.53418	2.088603	2.364066
+Xe	2	F	-1	4	1.77407	6.5	0.722521	2.0405	1.757469
+Sc	3	F	-1	6.255	1.65325	6	1.533224	1.913247	2.061856
+Ti	4	F	-1	6	1.6617	5.5	1.659907	1.748926	2.227171
+Fe	3	F	-1	5.733	1.63674	5	1.175592	1.791926	2.43309
+Co	3	F	-1	6	1.56345	5.5	1.395376	1.753918	2.257336
+Ni	2	F	-1	5.933	1.49655	5	1.10969	1.874661	2.212389
+Cu	2	F	-1	2.56	1.4953	5.5	1.423726	1.493666	2.188184
+Zn	2	F	-1	4.718	1.57447	5	0.925848	1.812843	2.463054
+Y	3	F	-1	7.285	1.89262	5.5	0.757641	2.11472	2.638522
+Zr	4	F	-1	6.765	1.83174	5.5	1.005776	1.927834	2.57732
+Nb	5	F	-1	6.044	1.76034	5.5	1.966109	1.751349	2.04499
+Rh	4	F	-1	6	1.68686	5.5	1.224679	1.733553	2.463054
+Pd	2	F	-1	4	1.56885	5.5	1.299983	1.793725	1.976285
+Ag	1	F	-1	4.438	1.58298	5	0.727114	2.196512	2.008032
+Cd	2	F	-1	6.176	1.73948	5.5	0.755986	2.084803	2.403846
+Lu	3	F	-1	6.83	1.80738	5.5	0.853953	2.023989	2.427184
+Hf	4	F	-1	7.105	1.7752	5.5	1.334791	1.937534	2.132196
+Ta	5	F	-1	6.09	1.79011	5.5	1.682167	1.778032	2.096436
+Au	3	F	-1	4	1.697	5.5	1.533484	1.706806	1.972387
+Hg	2	F	-1	6.966	1.7338	5.5	0.850135	2.187943	2.114165
+La	3	F	-1	9.83	1.96577	5.5	0.844511	2.366189	2.257336
+Pr	3	F	-1	9.067	1.91752	5.5	0.900775	2.268753	2.232143
+Nd	3	F	-1	8.647	1.91099	5.5	0.870992	2.232524	2.28833
+Ti	3	F	-1	6	1.6318	5.5	1.493295	1.829107	2.136752
+Cr	4	F	-1	5.429	1.64899	5	1.516679	1.658904	2.392344
+Fe	2	F	-1	5.743	1.50766	5.5	1.280077	1.902081	2.04499
+Ni	4	F	-1	6	1.61746	5.5	1.45655	1.670016	2.43309
+Cu	3	F	-1	4	1.54272	5.5	1.531932	1.554592	2.28833
+Nb	4	F	-1	6	1.75844	6	1.995819	1.840216	1.872659
+Ru	5	F	-1	6	1.77634	5.5	1.653541	1.724517	2.247191
+Rh	3	F	-1	6	1.63692	5.5	1.440772	1.843667	2.04918
+Pd	4	F	-1	5.333	1.68582	5.5	1.59323	1.688346	2.188184
+Ag	3	F	-1	6.25	1.71485	5.5	1.189009	1.916593	2.212389
+Pt	5	F	-1	6	1.78573	5.5	1.362673	1.734251	2.358491
+Hg	1	F	-1	4.786	1.76507	5.5	0.547747	2.401203	2.114165
+V	3	F	-1	6	1.61581	5.5	1.386802	1.804823	2.232143
+Cr	3	F	-1	6	1.58975	5.5	1.347343	1.775673	2.283105
+Co	2	F	-1	5.506	1.51442	5.5	1.155873	1.86403	2.173913
+Ni	3	F	-1	6	1.56869	5	1.275911	1.748854	2.364066
+Ag	2	F	-1	5	1.6378	5.5	1.195671	1.973406	1.964637
+Ta	3	F	-1	6	1.52314	6	1.747189	1.79512	1.801802
+Pt	4	F	-1	6	1.69132	5.5	1.597082	1.753192	2.04918
+V	2	F	-1	6	1.53303	5.5	1.232616	1.943136	2.061856
+Cr	2	F	-1	5.6	1.54102	5.5	1.26782	1.920471	2.04499
+Mn	4	F	-1	5.923	1.61606	5	1.45541	1.663202	2.439024
+Mo	3	F	-1	5.7	1.73819	5.5	1.078285	1.886081	2.34192
+Os	5	F	-1	6	1.75815	6	1.83525	1.705754	2.04918
+Mn	3	F	-1	5.862	1.59633	5.5	1.397213	1.775416	2.242152
+Mn	2	F	-1	5.91	1.56491	5.5	1.16586	1.962266	2.109705
+Ce	3	F	-1	9.147	1.92656	5.5	0.932803	2.289753	2.183406
+Sm	3	F	-1	8.119	1.88844	5.5	0.905474	2.187001	2.267574
+Eu	3	F	-1	7.743	1.87763	5.5	0.92616	2.15759	2.257336
+Gd	3	F	-1	8.052	1.90718	5.5	0.770786	2.177537	2.463054
+Tb	3	F	-1	7.958	1.83798	5.5	0.932919	2.132299	2.262443
+#Dy	3	F	-1	7.828	1.85	5.5	1.485846	1.296738	-2.298851
+Ho	3	F	-1	7.5	1.84485	5.5	0.871595	2.100218	2.358491
+Er	3	F	-1	7.135	1.84663	5.5	0.868164	2.078788	2.375297
+Tm	3	F	-1	6.912	1.81795	5.5	0.920982	2.044246	2.325581
+Yb	3	F	-1	6.875	1.80974	5.5	0.945748	2.037278	2.298851
+Eu	2	F	-1	10.111	1.8142	5.5	0.847162	2.482968	1.988072
+Th	4	F	-1	8.941	2.40121	7	1.270178	2.697147	1.782531
+Li	1	Cl	-1	5.258	1.39892	7	0.49302 	2.39647 	1.577287
+Be	2	Cl	-1	4	1.52729	6.5	1.323436	1.9291	1.517451
+#B	3	Cl	-1	3.417	1.675	6	2.579816	1.529824	-1.494768
+Na	1	Cl	-1	6.52	1.69489	6.5	0.315458	2.748011	1.663894
+Mg	2	Cl	-1	5.897	1.78276	6.5	0.796023	2.393298	1.587302
+Al	3	Cl	-1	5.327	1.89795	6.5	1.367335	2.197469	1.547988
+P	5	Cl	-1	4	2.01093	7	2.935183	1.791686	1.510574
+K	1	Cl	-1	8.846	2.07673	6.5	0.201068	3.184081	1.801802
+Ca	2	Cl	-1	7.544	2.06262	6.5	0.53146	2.759777	1.683502
+Ga	3	Cl	-1	4.905	1.97794	6.5	0.959766	2.170468	1.730104
+Ge	4	Cl	-1	4.305	2.07619	6	1.521374	2.033413	1.639344
+Rb	1	Cl	-1	10.02	2.26585	6.5	0.155502	3.370857	1.883239
+Sr	2	Cl	-1	9.4	2.20197	6.5	0.408921	2.985294	1.745201
+In	3	Cl	-1	6.024	2.13474	6.5	0.695073	2.409564	1.824818
+Sn	4	Cl	-1	6.069	2.17643	6.5	1.106595	2.32334	1.70068
+Sb	5	Cl	-1	6	2.2232	6.5	1.572233	2.243372	1.623377
+Cs	1	Cl	-1	11.79	2.46037	6.5	0.119331	3.555351	2
+Ba	2	Cl	-1	10.32	2.41041	6.5	0.290875	3.143075	1.926782
+Tl	3	Cl	-1	5.22	2.22567	6	0.56302	2.389021	1.945525
+S	4	Cl	-1	3	2.05269	6.5	1.591239	1.791962	1.834862
+Ga	1	Cl	-1	4.905	2.3204	6	0.14014	2.871349	2.272727
+As	3	Cl	-1	3	2.06175	6	0.870752	1.951235	1.915709
+Se	4	Cl	-1	3	2.15849	6.5	1.304935	1.89237	1.834862
+In	1	Cl	-1	6.024	2.43863	6	0.105153	3.015535	2.421308
+Sb	3	Cl	-1	6	2.30831	6	0.544277	2.520874	2.016129
+Te	4	Cl	-1	3.396	2.30563	6.5	0.951857	2.09621	1.930502
+Tl	1	Cl	-1	8.03	2.36792	6	0.126355	3.237936	2.03666
+Pb	2	Cl	-1	7.541	2.34641	5.5	0.268937	2.83552	2.109705
+Bi	3	Cl	-1	6.058	2.34105	6	0.50612	2.565353	1.980198
+Sc	3	Cl	-1	6.255	2.1133	6.5	1.541393	2.474212	1.633987
+Ti	4	Cl	-1	6	2.12577	6	1.346432	2.244649	1.972387
+#Cr	6	Cl	-1	4	2.007	6.5	2.648568	2.185395	-1.577287
+Fe	3	Cl	-1	5.733	1.98266	6	1.322259	2.228926	1.858736
+Ni	2	Cl	-1	5.933	1.87666	5.5	0.825239	2.282632	2.10084
+Cu	2	Cl	-1	2.56	1.90175	5.5	0.964976	1.903186	2.12766
+Zn	2	Cl	-1	4.718	1.88195	6	1.012812	2.228172	1.919386
+Y	3	Cl	-1	7.285	2.28867	6.5	0.812042	2.616424	2.070393
+Zr	4	Cl	-1	6.765	2.18437	6.5	1.61247	2.41089	1.644737
+Nb	5	Cl	-1	6.044	2.20986	6.5	1.996217	2.234964	1.623377
+#Mo	6	Cl	-1	4.764	2.0888	6.5	2.320539	2.147333	-1.607717
+Pd	2	Cl	-1	4	1.99818	5	0.61099	2.157132	2.375297
+Ag	1	Cl	-1	4.438	1.98819	5	0.387504	2.497296	2.331002
+Cd	2	Cl	-1	6.176	2.0695	6	0.769487	2.533294	1.953125
+Lu	3	Cl	-1	6.83	2.284	6	0.617863	2.522817	2.309469
+Hf	4	Cl	-1	7.105	2.2444	6.5	0.924292	2.423017	2.070393
+Ta	5	Cl	-1	6.09	2.21442	6.5	1.749379	2.23829	1.655629
+W	6	Cl	-1	5.688	2.21497	7	2.141315	2.09029	1.620746
+Pt	2	Cl	-1	4	1.97699	5.5	0.65892	2.142168	2.192982
+Au	3	Cl	-1	4	2.14532	5.5	0.69387	2.123675	2.375297
+Hg	2	Cl	-1	6.966	2.17009	5.5	0.539918	2.602861	2.197802
+La	3	Cl	-1	9.83	2.43099	6	0.612367	2.860323	2.178649
+Pr	3	Cl	-1	9.067	2.48619	5.5	0.449895	2.767658	2.583979
+Ti	3	Cl	-1	6	2.13089	6	0.925547	2.317792	2.178649
+Fe	2	Cl	-1	5.743	2.00003	5	0.686296	2.334636	2.277904
+Rh	3	Cl	-1	6	2.03722	5	0.797203	2.211713	2.272727
+Pd	4	Cl	-1	5.333	2.12662	6	1.088684	2.133809	2.12766
+W	5	Cl	-1	6	2.24489	6	0.871662	2.172085	2.380952
+Hg	1	Cl	-1	4.786	2.17341	5.5	0.365096	2.721804	2.197802
+Ti	2	Cl	-1	6	2.03427	5.5	0.644954	2.372399	2.331002
+V	3	Cl	-1	6	2.06334	5.5	1.031449	2.274479	2.083333
+Cr	3	Cl	-1	6	2.0051	5.5	1.092685	2.228283	2.04499
+Co	2	Cl	-1	5.506	1.93137	5.5	0.795676	2.288535	2.136752
+Cu	1	Cl	-1	2.56	1.79822	5	0.462969	2.052044	2.487562
+Zr	2	Cl	-1	6.765	2.12072	6	0.670128	2.53539	2.09205
+Mo	4	Cl	-1	6	2.1283	6.5	1.489813	2.197852	1.792115
+Ir	3	Cl	-1	6	2.05823	5.5	0.612349	2.194093	2.487562
+Pt	4	Cl	-1	6	2.1411	6	0.851686	2.182212	2.272727
+V	2	Cl	-1	6	2.03267	5.5	0.679979	2.388641	2.262443
+Cr	2	Cl	-1	5.6	2.01499	5.5	0.685419	2.337625	2.277904
+Mn	4	Cl	-1	5.923	2.06541	6.5	1.457267	2.156547	1.934236
+Mo	3	Cl	-1	5.7	2.08941	6	0.996785	2.293329	1.996008
+Tc	4	Cl	-1	6	2.15861	6	1.046765	2.219262	2.12766
+Ru	3	Cl	-1	6	1.9952	5.5	0.981474	2.218867	2.04499
+W	3	Cl	-1	6	2.12237	5	0.672476	2.264711	2.336449
+Re	4	Cl	-1	6	2.18513	5.5	0.739216	2.204421	2.427184
+Mo	2	Cl	-1	5.5	2.05175	5.5	0.616601	2.345416	2.267574
+Os	4	Cl	-1	6	2.15572	6	0.779449	2.182969	2.375297
+Mn	2	Cl	-1	5.91	1.99681	6	0.821608	2.409777	2.04918
+Re	3	Cl	-1	6	2.15781	5.5	0.639211	2.294331	2.380952
+Eu	3	Cl	-1	7.743	2.31998	6	0.739494	2.644542	2.061856
+Gd	3	Cl	-1	8.052	2.27126	6	0.881597	2.679082	1.876173
+Tb	3	Cl	-1	7.958	2.29526	6	0.745002	2.635827	2.057613
+Dy	3	Cl	-1	7.828	2.2881	6	0.768339	2.629921	2.028398
+Er	3	Cl	-1	7.135	2.25982	6	0.830373	2.573621	1.972387
+Yb	2	Cl	-1	8	2.29464	5.5	0.419744	2.705315	2.444988
+Eu	2	Cl	-1	10.111	2.41447	5.5	0.416527	2.943683	2.352941
+Li	1	Br	-1	5.263	1.51288	7	0.44910 	2.58255 	1.481481
+#Be	2	Br	-1	4	1.6581	7	2.215989	1.122546	-1.430615
+#B	3	Br	-1	3.417	1.821	6.5	2.291796	1.675041	-1.410437
+Na	1	Br	-1	6.52	1.78228	7	0.292879	2.915883	1.560062
+Mg	2	Br	-1	5.897	1.89059	7	0.733669	2.551036	1.490313
+Al	3	Br	-1	5.327	2.04045	7	1.242373	2.36878	1.455604
+K	1	Br	-1	8.846	2.17206	7	0.188913	3.373219	1.680672
+#Ca	2	Br	-1	7.544	2.1686	7	1.165036	1.242057	-1.577287
+Ga	3	Br	-1	4.905	2.11352	6.5	0.887656	2.330935	1.615509
+Rb	1	Br	-1	10.02	2.34362	7	0.14833	3.55125	1.748252
+#Sr	2	Br	-1	9.4	2.3125	7	0.95906	1.265723	-1.628664
+In	3	Br	-1	6.024	2.28936	6.5	0.645222	2.596929	1.697793
+Cs	1	Br	-1	11.79	2.50818	7	0.115797	3.714691	1.848429
+#Ba	2	Br	-1	10.32	2.486	7	0.74336	1.399882	-1.680672
+Tl	3	Br	-1	5.22	2.35992	6	0.532392	2.550956	1.801802
+Se	4	Br	-1	3	2.32723	7	1.200099	2.05318	1.709402
+In	1	Br	-1	6.024	2.46665	6	0.106082	3.128138	2.202643
+Sb	3	Br	-1	6	2.38165	7	0.529405	2.630872	1.862197
+Te	4	Br	-1	3.396	2.46108	7	0.894624	2.249368	1.788909
+Tl	1	Br	-1	8.03	2.42772	6	0.102033	3.27736	2.096436
+Pb	2	Br	-1	7.541	2.4316	6	0.261373	2.982711	1.941748
+Bi	3	Br	-1	6.058	2.46708	7	0.480534	2.725316	1.834862
+#Cr	6	Br	-1	4	2.224	6.5	2.339341	2.421694	-1.48368
+Fe	3	Br	-1	5.733	2.13627	6.5	1.22157	2.411656	1.730104
+Ni	2	Br	-1	5.933	1.96729	6	0.791638	2.421615	1.937984
+Zn	2	Br	-1	4.718	1.98741	6	0.958104	2.373518	1.779359
+Y	3	Br	-1	7.285	2.40922	6.5	0.7734	2.778819	1.915709
+Zr	4	Br	-1	6.765	2.32815	7	1.481279	2.581699	1.54321
+#Mo	6	Br	-1	4.764	2.3037	6.5	2.064478	2.374953	-1.508296
+Pd	2	Br	-1	4	2.10183	5.5	0.599388	2.293259	2.164502
+Ag	1	Br	-1	4.438	2.03699	5.5	0.384726	2.614612	2.12766
+Cd	2	Br	-1	6.176	2.16913	6	0.733475	2.684989	1.808318
+Au	3	Br	-1	4	2.27911	5.5	0.673499	2.271943	2.169197
+Hg	2	Br	-1	6.966	2.25138	6	0.525569	2.740738	2.020202
+Fe	2	Br	-1	5.743	2.09517	5.5	0.666987	2.476774	2.087683
+Ti	2	Br	-1	6	2.15487	6	0.625835	2.541373	2.12766
+Cr	3	Br	-1	6	2.13165	6.5	1.037691	2.387051	1.886792
+Cu	1	Br	-1	2.56	1.8681	5.5	0.459534	2.164436	2.262443
+W	4	Br	-1	6	2.3517	6.5	0.67355	2.378816	2.277904
+V	2	Br	-1	6	2.10218	6	0.669272	2.509714	2.070393
+Cr	2	Br	-1	5.6	2.12678	6	0.66474	2.495533	2.083333
+Mo	3	Br	-1	5.7	2.19147	6	0.951252	2.426733	1.848429
+Mo	2	Br	-1	5.5	2.22218	5.5	0.418518	2.474296	2.493766
+W	2	Br	-1	6	1.95717	7	0.966423	2.546409	1.545595
+Os	4	Br	-1	6	2.30615	6	0.751339	2.351622	2.169197
+Mn	2	Br	-1	5.91	2.08701	6	0.787476	2.54896	1.893939
+Re	3	Br	-1	6	2.30419	5.5	0.524717	2.443614	2.369668
+Eu	2	Br	-1	10.111	2.50011	6	0.409845	3.10151	2.150538
+Li	1	I	-1	5.000	1.64829	7	0.44117	        2.78807 	1.360544
+#Be	2	I	-1	4	1.8008	7	2.134019	1.232513	-1.315789
+#B	3	I	-1	3.417	2.007	7	2.173632	1.863156	-1.298701
+Na	1	I	-1	6.52	1.94353	7	0.285612	3.198502	1.426534
+#Mg	2	I	-1	5.897	2.045	7	1.655681	1.199982	-1.367989
+Al	3	I	-1	5.327	2.24648	7	1.187824	2.619974	1.338688
+P	5	I	-1	4	2.49792	7.5	2.382629	2.27117	1.310616
+K	1	I	-1	8.846	2.2888	7	0.190106	3.633321	1.526718
+#Ca	2	I	-1	7.544	2.3242	7	1.170657	1.328579	-1.438849
+#Ga	3	I	-1	4.905	2.314	7	1.170186	1.902933	-1.472754
+Rb	1	I	-1	10.02	2.46445	7	0.150421	3.823732	1.582278
+#Sr	2	I	-1	9.4	2.3242	7	1.189417	1.169575	-1.438849
+In	3	I	-1	6.024	2.47773	7	0.674268	2.850379	1.49925
+Cs	1	I	-1	11.79	2.71194	8	0.116459	4.07706	1.663894
+#Ba	2	I	-1	10.32	2.6495	7.5	0.763038	1.478218	-1.526718
+Ga	1	I	-1	4.905	2.38769	7	0.150745	3.125864	1.848429
+In	1	I	-1	6.024	2.50769	7	0.115503	3.293778	1.945525
+Sb	3	I	-1	6	2.59905	7.5	0.531155	2.898754	1.675042
+Te	4	I	-1	3.396	2.67663	7.5	0.895233	2.465289	1.615509
+Tl	1	I	-1	8.03	2.48689	7	0.109014	3.477263	1.862197
+Pb	2	I	-1	7.541	2.5688	7	0.270625	3.211959	1.73913
+Bi	3	I	-1	6.058	2.63989	7.5	0.488978	2.951989	1.652893
+#Cr	6	I	-1	4	2.5373	7	2.176374	2.768722	-1.360544
+Fe	3	I	-1	5.733	2.37658	6	0.822293	2.623615	1.912046
+Zn	2	I	-1	4.718	2.15151	6.5	0.959066	2.597824	1.607717
+#Mo	6	I	-1	4.764	2.6191	7	1.922048	2.713286	-1.383126
+Ag	1	I	-1	4.438	2.08036	6	0.414392	2.760885	1.886792
+Cd	2	I	-1	6.176	2.3244	7	0.741701	2.918199	1.631321
+Hf	4	I	-1	7.105	2.57677	7	0.895483	2.832144	1.712329
+Hg	2	I	-1	6.966	2.38163	6	0.547753	2.956874	1.801802
+Fe	2	I	-1	5.743	2.25785	6	0.692512	2.711676	1.851852
+Zr	3	I	-1	6.765	2.56625	6	0.562056	2.796227	2.118644
+Co	2	I	-1	5.506	2.19837	6	0.780849	2.670145	1.757469
+Cu	1	I	-1	2.56	1.93067	6	0.501948	2.295302	1.988072
+Zr	2	I	-1	6.765	2.49296	5.5	0.36402	2.844654	2.358491
+Cr	2	I	-1	5.6	2.28404	6.5	0.689638	2.722975	1.851852
+Mo	2	I	-1	5.5	2.35705	6	0.456968	2.678791	2.169197
+Mn	2	I	-1	5.91	2.26045	6.5	0.796403	2.795756	1.70068
+Eu	2	I	-1	10.111	2.66292	6.5	0.429764	3.372258	1.904762
+Li	1	N	-3	5.021	1.1543	6	2.054953	2.132557	1.569859
+Mg	2	N	-3	5.897	1.63729	6	2.874771	2.215919	1.663894
+Sr	2	N	-3	9.4	2.09477	6.5	1.428465	2.830165	1.838235
+Cr	6	N	-3	4	1.96859	6.5	6.823816	1.638522	1.652893
+Nb	5	N	-3	6.044	2.0288	5	2.833875	2.027799	2.083333
+Eu	3	N	-3	7.743	2.1627	6	1.484427	2.459643	2.197802
+Gd	3	N	-3	8.052	2.09519	6.5	1.809718	2.475474	1.984127
+Eu	2	N	-3	10.111	2.1874	6	0.974842	2.731273	2.325581
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/elements.dat` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/elements.dat`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-1	H	1	1	1.0079	1	1	0	0.37	0
-3	Li	1	1	6.941	2	1	1	1.31	0.02847
-4	Be	2	2	9.0122	2	2	1	0.91	0.01474
-5	B	3	3	10.811	2	3	1	0.71	0.00903
-6	C	2	4	12.0107	2	4	1	0.77	0.08509
-6	C	3	4	12.0107	2	4	1	0.77	0.08509
-6	C	4	4	12.0107	2	4	1	0.77	0.00611
-6	C	-2	4	12.0107	2	4	1	0	0
-7	N	-3	5	14.0067	2	5	1	1.32	0.197
-7	N	3	5	14.0067	2	5	1	0.74	0.06661
-7	N	5	5	14.0067	2	5	1	0.74	0.0044
-8	O	-2	-2	15.9994	2	6	1	1.33	0.14752
-8	O	6	-2	15.9994	2	6	1	0.74	0.00333
-9	F	-1	-1	18.9994	2	7	1	1.26	0.14262
-11	Na	1	1	22.9898	3	1	1	1.66	0.04746
-12	Mg	2	2	24.305	3	2	1	1.36	0.03072
-13	Al	3	3	26.9815	3	3	1	1.11	0.02185
-14	Si	4	4	28.0855	3	4	1	1.17	0.01644
-15	P	3	5	30.9738	3	5	1	1.1	0.09416
-15	P	5	5	30.9738	3	5	1	1.1	0.01287
-16	S	-2	-2	32.066	3	6	1	1.77	0.22433
-16	S	4	-2	32.066	3	6	1	1.04	0.07882
-16	S	6	-2	32.066	3	6	1	1.04	0.01037
-17	Cl	-1	-1	35.4527	3	7	1	1.74	0.21389
-17	Cl	3	-1	35.4527	3	7	1	0.99	0.14437
-17	Cl	5	-1	35.4527	3	7	1	0.99	0.07909
-17	Cl	7	-1	35.4527	3	7	1	0.99	0.00854
-18	Ar	0	0	39.948	3	8	1	0	0.99999
-19	K	1	1	39.0983	4	1	1	2.06	0.07328
-20	Ca	2	2	40.078	4	2	1	1.66	0.05123
-21	Sc	3	3	44.9559	4	3	2	1.46	0.04104
-22	Ti	2	4	47.867	4	4	2	1.26	0.14372
-22	Ti	3	4	47.867	4	4	2	1.26	0.12678
-22	Ti	4	4	47.867	4	4	2	1.26	0.03569
-23	V	2	5	50.9415	4	5	2	1.21	0.13628
-23	V	3	5	50.9415	4	5	2	1.21	0.11507
-23	V	4	5	50.9415	4	5	2	1.21	0.1077
-23	V	5	5	50.9415	4	5	2	1.21	0.03182
-24	Cr	2	6	51.9961	4	6	2	1.21	0.13819
-24	Cr	3	6	51.9961	4	6	2	1.21	0.10989
-24	Cr	4	6	51.9961	4	6	2	1.21	0.0985
-24	Cr	5	6	51.9961	4	6	2	1.21	0.09446
-24	Cr	6	6	51.9961	4	6	2	1.21	0.02876
-25	Mn	2	7	54.938	4	7	2	1.26	0.11097
-25	Mn	3	7	54.938	4	7	2	1.26	0.11405
-25	Mn	4	7	54.938	4	7	2	1.26	0.09413
-25	Mn	5	7	54.938	4	7	2	1.26	0.08653
-25	Mn	6	7	54.938	4	7	2	1.26	0.08464
-25	Mn	7	7	54.938	4	7	2	1.26	0.02654
-26	Fe	2	3	55.845	4	8	2	1.26	0.13832
-26	Fe	3	3	55.845	4	8	2	1.26	0.08271
-26	Fe	4	3	55.845	4	8	2	1.26	0.04856
-27	Co	1	3	58.9332	4	8	2	1.21	0.21741
-27	Co	2	3	58.9332	4	8	2	1.21	0.12182
-27	Co	3	3	58.9332	4	8	2	1.21	0.11232
-27	Co	4	3	58.9332	4	8	2	1.21	0.07094
-28	Ni	2	2	58.6934	4	8	2	1.21	0.11752
-28	Ni	3	2	58.6934	4	8	2	1.21	0.1013
-28	Ni	4	2	58.6934	4	8	2	1.21	0.09464
-29	Cu	1	2	63.546	4	1	2	1.21	0.15914
-29	Cu	2	2	63.546	4	1	2	1.21	0.12091
-29	Cu	3	2	63.546	4	1	2	1.21	0.1089
-30	Zn	2	2	65.39	4	2	2	1.21	0.0919
-31	Ga	1	3	69.723	4	3	1	1.16	0.13779
-31	Ga	3	3	69.723	4	3	1	1.16	0.05998
-32	Ge	2	4	72.61	4	4	1	1.22	0.10936
-32	Ge	4	4	72.61	4	4	1	1.22	0.04187
-33	As	3	5	74.922	4	5	1	1.21	0.0918
-33	As	5	5	74.9216	4	5	1	1.21	0.03079
-34	Se	-2	6	78.96	4	6	1	1.91	0.24167
-34	Se	4	6	78.96	4	6	1	1.17	0.07889
-34	Se	6	6	78.96	4	6	1	1.17	0.02714
-34	Se	-1	6	78.96	4	6	1	1.91	0
-35	Br	-1	-1	79.904	4	7	1	1.89	0.23669
-35	Br	5	-1	79.904	4	7	1	1.14	0.06916
-35	Br	7	-1	79.904	4	7	1	1.14	0.02228
-36	Kr	0	0	83.8	4	8	1	0	0.99999
-37	Rb	1	1	85.4678	5	1	1	2.21	0.08653
-38	Sr	2	2	87.62	5	2	1	1.86	0.06278
-39	Y	3	3	88.9059	5	3	2	1.66	0.0499
-40	Zr	2	4	91.224	5	4	2	1.41	0.20355
-40	Zr	3	4	91.224	5	4	2	1.41	0.17623
-40	Zr	4	4	91.224	5	4	2	1.41	0.04347
-41	Nb	2	5	92.9064	5	5	2	1.31	0.18626
-41	Nb	3	5	92.9064	5	5	2	1.31	0.15029
-41	Nb	4	5	92.9064	5	5	2	1.31	0.16395
-41	Nb	5	5	92.9064	5	5	2	1.31	0.03883
-42	Mo	2	6	95.94	5	6	2	1.31	0.18239
-42	Mo	3	6	95.94	5	6	2	1.31	0.10364
-42	Mo	4	6	95.94	5	6	2	1.31	0.24835
-42	Mo	5	6	95.94	5	6	2	1.31	0.13945
-42	Mo	6	6	95.94	5	6	2	1.31	0.03519
-43	Tc	4	7	98	5	7	2	1.21	0.12061
-43	Tc	7	7	98	5	7	2	1.21	0.02969
-44	Ru	3	6	101.07	5	8	2	1.16	0.11008
-44	Ru	4	6	101.07	5	8	2	1.16	0.12061
-44	Ru	5	6	101.07	5	8	2	1.16	0.11351
-44	Ru	6	6	101.07	5	8	2	1.16	0.10721
-45	Rh	3	4	102.906	5	8	2	1.21	0.13754
-45	Rh	4	4	102.906	5	8	2	1.21	0.09189
-46	Pd	2	2	106.42	5	8	2	1.26	0.14821
-46	Pd	4	2	106.42	5	8	2	1.26	0.12061
-47	Ag	1	1	107.868	5	1	2	1.46	0.14379
-47	Ag	2	1	107.868	5	1	2	1.46	0.14982
-47	Ag	3	1	107.868	5	1	2	1.46	0.11774
-48	Cd	2	2	112.411	5	2	2	1.41	0.09723
-49	In	1	3	114.818	5	3	1	1.41	0.15286
-49	In	3	3	114.818	5	3	1	1.41	0.077
-50	Sn	2	4	118.7	5	4	1	1.4	0.12603
-50	Sn	4	4	118.71	5	4	1	1.4	0.05473
-51	Sb	3	5	121.76	5	5	1	1.41	0.10603
-51	Sb	5	5	121.76	5	5	1	1.41	0.03859
-52	Te	-2	6	127.6	5	6	1	2.14	0.26716
-52	Te	2	6	127.6	5	6	1	1.37	0.21252
-52	Te	4	6	127.6	5	6	1	1.37	0.09377
-52	Te	6	6	127.6	5	6	1	1.37	0.03025
-53	I	-1	-1	126.904	5	7	1	2.13	0.27057
-53	I	5	-1	126.904	5	7	1	1.33	0.0804
-53	I	7	-1	126.904	5	7	1	1.33	0.02506
-54	Xe	2	0	131.29	5	8	1	1.3	0.18361
-54	Xe	4	0	131.29	5	8	1	1.3	0.16081
-54	Xe	6	0	131.29	5	8	1	1.3	0.07147
-55	Cs	1	1	132.905	6	1	1	2.46	0.10383
-56	Ba	2	2	137.327	6	2	1	2.01	0.07324
-57	La	3	3	138.906	6	0	3	1.81	0.065
-58	Ce	3	4	140.116	6	0	3	1.71	0.12076
-58	Ce	4	4	140.116	6	0	3	1.71	0.06946
-59	Pr	3	3	140.908	6	0	3	1.71	0.11521
-60	Nd	3	3	144.24	6	0	3	1.71	0.10902
-62	Sm	3	3	150.36	6	0	3	1.71	0.11154
-63	Eu	2	3	151.964	6	0	3	1.71	0.1463
-63	Eu	3	3	151.964	6	0	3	1.71	0.11245
-64	Gd	3	3	157.25	6	0	3	1.66	0.08538
-65	Tb	3	3	158.9254	6	0	3	1.61	0.11187
-65	Tb	4	3	158.9254	6	0	3	1.61	0.99999
-66	Dy	3	3	162.5	6	0	3	1.61	0.1078
-67	Ho	3	3	164.9303	6	0	3	1.61	0.10178
-68	Er	3	3	167.259	6	0	3	1.61	0.10019
-69	Tm	3	3	168.9342	6	0	3	1.61	0.10516
-70	Yb	2	3	173.0545	6	0	3	1.61	0.15535
-70	Yb	3	3	173.0545	6	0	3	1.61	0.10805
-71	Lu	3	3	174.967	6	3	2	1.61	0.0822
-72	Hf	4	4	178.49	6	4	2	1.41	0.05
-73	Ta	2	5	180.949	6	5	2	1.31	0.32162
-73	Ta	3	5	180.949	6	5	2	1.31	0.17543
-73	Ta	4	5	112.411	6	5	2	1.31	0.17543
-73	Ta	5	5	180.948	6	5	2	1.31	0.04545
-74	W	2	6	183.84	6	6	2	1.21	0.32154
-74	W	3	6	183.84	6	6	2	1.21	0.17544
-74	W	4	6	183.84	6	6	2	1.21	0.1608
-74	W	5	6	183.84	6	6	2	1.21	0.14843
-74	W	6	6	183.84	6	6	2	1.21	0.03846
-75	Re	3	7	186.207	6	7	2	1.21	0.17077
-75	Re	4	7	186.207	6	7	2	1.21	0.15315
-75	Re	5	7	186.207	6	7	2	1.21	0.13784
-75	Re	6	7	186.207	6	7	2	1.21	0.14844
-75	Re	7	7	186.207	6	7	2	1.21	0.03333
-76	Os	4	8	190.23	6	8	2	1.16	0.14844
-76	Os	5	8	190.23	6	8	2	1.16	0.13784
-76	Os	6	8	190.23	6	8	2	1.16	0.12865
-76	Os	7	8	190.23	6	8	2	1.16	0.13784
-76	Os	8	8	190.23	6	8	2	1.16	0.0303
-77	Ir	3	5	192.217	6	8	2	1.21	0.16081
-77	Ir	4	5	192.217	6	8	2	1.21	0.11351
-77	Ir	5	5	192.217	6	8	2	1.21	0.13784
-78	Pt	2	2	195.078	6	8	2	1.21	0.19125
-78	Pt	3	2	195.078	6	8	2	1.21	0.17543
-78	Pt	4	2	195.078	6	8	2	1.21	0.13784
-78	Pt	5	2	195.078	6	8	2	1.21	0.10156
-79	Au	1	3	196.967	6	1	2	1.21	0.17705
-79	Au	3	3	196.967	6	1	2	1.21	0.14844
-80	Hg	1	2	200.59	6	2	2	1.36	0.24034
-80	Hg	2	2	200.59	6	2	2	1.36	0.12951
-81	Tl	1	3	204.383	6	3	1	1.76	0.13967
-81	Tl	3	3	204.383	6	3	1	1.76	0.09582
-82	Pb	2	4	207.2	6	4	1	1.66	0.11831
-82	Pb	4	4	207.2	6	4	1	1.66	0.07547
-83	Bi	3	5	208.98	6	5	1	1.46	0.10135
-83	Bi	5	5	208.98	6	5	1	1.46	0.06185
-90	Th	4	4	232.04	7	0	3	1.66	0.069
-92	U	6	6	238.03	7	0	3	1.61	0.03
+1	H	1	1	1.0079	1	1	0	0.37	0
+3	Li	1	1	6.941	2	1	1	1.31	0.02847
+4	Be	2	2	9.0122	2	2	1	0.91	0.01474
+5	B	3	3	10.811	2	3	1	0.71	0.00903
+6	C	2	4	12.0107	2	4	1	0.77	0.08509
+6	C	3	4	12.0107	2	4	1	0.77	0.08509
+6	C	4	4	12.0107	2	4	1	0.77	0.00611
+6	C	-2	4	12.0107	2	4	1	0	0
+7	N	-3	5	14.0067	2	5	1	1.32	0.197
+7	N	3	5	14.0067	2	5	1	0.74	0.06661
+7	N	5	5	14.0067	2	5	1	0.74	0.0044
+8	O	-2	-2	15.9994	2	6	1	1.33	0.14752
+8	O	6	-2	15.9994	2	6	1	0.74	0.00333
+9	F	-1	-1	18.9994	2	7	1	1.26	0.14262
+11	Na	1	1	22.9898	3	1	1	1.66	0.04746
+12	Mg	2	2	24.305	3	2	1	1.36	0.03072
+13	Al	3	3	26.9815	3	3	1	1.11	0.02185
+14	Si	4	4	28.0855	3	4	1	1.17	0.01644
+15	P	3	5	30.9738	3	5	1	1.1	0.09416
+15	P	5	5	30.9738	3	5	1	1.1	0.01287
+16	S	-2	-2	32.066	3	6	1	1.77	0.22433
+16	S	4	-2	32.066	3	6	1	1.04	0.07882
+16	S	6	-2	32.066	3	6	1	1.04	0.01037
+17	Cl	-1	-1	35.4527	3	7	1	1.74	0.21389
+17	Cl	3	-1	35.4527	3	7	1	0.99	0.14437
+17	Cl	5	-1	35.4527	3	7	1	0.99	0.07909
+17	Cl	7	-1	35.4527	3	7	1	0.99	0.00854
+18	Ar	0	0	39.948	3	8	1	0	0.99999
+19	K	1	1	39.0983	4	1	1	2.06	0.07328
+20	Ca	2	2	40.078	4	2	1	1.66	0.05123
+21	Sc	3	3	44.9559	4	3	2	1.46	0.04104
+22	Ti	2	4	47.867	4	4	2	1.26	0.14372
+22	Ti	3	4	47.867	4	4	2	1.26	0.12678
+22	Ti	4	4	47.867	4	4	2	1.26	0.03569
+23	V	2	5	50.9415	4	5	2	1.21	0.13628
+23	V	3	5	50.9415	4	5	2	1.21	0.11507
+23	V	4	5	50.9415	4	5	2	1.21	0.1077
+23	V	5	5	50.9415	4	5	2	1.21	0.03182
+24	Cr	2	6	51.9961	4	6	2	1.21	0.13819
+24	Cr	3	6	51.9961	4	6	2	1.21	0.10989
+24	Cr	4	6	51.9961	4	6	2	1.21	0.0985
+24	Cr	5	6	51.9961	4	6	2	1.21	0.09446
+24	Cr	6	6	51.9961	4	6	2	1.21	0.02876
+25	Mn	2	7	54.938	4	7	2	1.26	0.11097
+25	Mn	3	7	54.938	4	7	2	1.26	0.11405
+25	Mn	4	7	54.938	4	7	2	1.26	0.09413
+25	Mn	5	7	54.938	4	7	2	1.26	0.08653
+25	Mn	6	7	54.938	4	7	2	1.26	0.08464
+25	Mn	7	7	54.938	4	7	2	1.26	0.02654
+26	Fe	2	3	55.845	4	8	2	1.26	0.13832
+26	Fe	3	3	55.845	4	8	2	1.26	0.08271
+26	Fe	4	3	55.845	4	8	2	1.26	0.04856
+27	Co	1	3	58.9332	4	8	2	1.21	0.21741
+27	Co	2	3	58.9332	4	8	2	1.21	0.12182
+27	Co	3	3	58.9332	4	8	2	1.21	0.11232
+27	Co	4	3	58.9332	4	8	2	1.21	0.07094
+28	Ni	2	2	58.6934	4	8	2	1.21	0.11752
+28	Ni	3	2	58.6934	4	8	2	1.21	0.1013
+28	Ni	4	2	58.6934	4	8	2	1.21	0.09464
+29	Cu	1	2	63.546	4	1	2	1.21	0.15914
+29	Cu	2	2	63.546	4	1	2	1.21	0.12091
+29	Cu	3	2	63.546	4	1	2	1.21	0.1089
+30	Zn	2	2	65.39	4	2	2	1.21	0.0919
+31	Ga	1	3	69.723	4	3	1	1.16	0.13779
+31	Ga	3	3	69.723	4	3	1	1.16	0.05998
+32	Ge	2	4	72.61	4	4	1	1.22	0.10936
+32	Ge	4	4	72.61	4	4	1	1.22	0.04187
+33	As	3	5	74.922	4	5	1	1.21	0.0918
+33	As	5	5	74.9216	4	5	1	1.21	0.03079
+34	Se	-2	6	78.96	4	6	1	1.91	0.24167
+34	Se	4	6	78.96	4	6	1	1.17	0.07889
+34	Se	6	6	78.96	4	6	1	1.17	0.02714
+34	Se	-1	6	78.96	4	6	1	1.91	0
+35	Br	-1	-1	79.904	4	7	1	1.89	0.23669
+35	Br	5	-1	79.904	4	7	1	1.14	0.06916
+35	Br	7	-1	79.904	4	7	1	1.14	0.02228
+36	Kr	0	0	83.8	4	8	1	0	0.99999
+37	Rb	1	1	85.4678	5	1	1	2.21	0.08653
+38	Sr	2	2	87.62	5	2	1	1.86	0.06278
+39	Y	3	3	88.9059	5	3	2	1.66	0.0499
+40	Zr	2	4	91.224	5	4	2	1.41	0.20355
+40	Zr	3	4	91.224	5	4	2	1.41	0.17623
+40	Zr	4	4	91.224	5	4	2	1.41	0.04347
+41	Nb	2	5	92.9064	5	5	2	1.31	0.18626
+41	Nb	3	5	92.9064	5	5	2	1.31	0.15029
+41	Nb	4	5	92.9064	5	5	2	1.31	0.16395
+41	Nb	5	5	92.9064	5	5	2	1.31	0.03883
+42	Mo	2	6	95.94	5	6	2	1.31	0.18239
+42	Mo	3	6	95.94	5	6	2	1.31	0.10364
+42	Mo	4	6	95.94	5	6	2	1.31	0.24835
+42	Mo	5	6	95.94	5	6	2	1.31	0.13945
+42	Mo	6	6	95.94	5	6	2	1.31	0.03519
+43	Tc	4	7	98	5	7	2	1.21	0.12061
+43	Tc	7	7	98	5	7	2	1.21	0.02969
+44	Ru	3	6	101.07	5	8	2	1.16	0.11008
+44	Ru	4	6	101.07	5	8	2	1.16	0.12061
+44	Ru	5	6	101.07	5	8	2	1.16	0.11351
+44	Ru	6	6	101.07	5	8	2	1.16	0.10721
+45	Rh	3	4	102.906	5	8	2	1.21	0.13754
+45	Rh	4	4	102.906	5	8	2	1.21	0.09189
+46	Pd	2	2	106.42	5	8	2	1.26	0.14821
+46	Pd	4	2	106.42	5	8	2	1.26	0.12061
+47	Ag	1	1	107.868	5	1	2	1.46	0.14379
+47	Ag	2	1	107.868	5	1	2	1.46	0.14982
+47	Ag	3	1	107.868	5	1	2	1.46	0.11774
+48	Cd	2	2	112.411	5	2	2	1.41	0.09723
+49	In	1	3	114.818	5	3	1	1.41	0.15286
+49	In	3	3	114.818	5	3	1	1.41	0.077
+50	Sn	2	4	118.7	5	4	1	1.4	0.12603
+50	Sn	4	4	118.71	5	4	1	1.4	0.05473
+51	Sb	3	5	121.76	5	5	1	1.41	0.10603
+51	Sb	5	5	121.76	5	5	1	1.41	0.03859
+52	Te	-2	6	127.6	5	6	1	2.14	0.26716
+52	Te	2	6	127.6	5	6	1	1.37	0.21252
+52	Te	4	6	127.6	5	6	1	1.37	0.09377
+52	Te	6	6	127.6	5	6	1	1.37	0.03025
+53	I	-1	-1	126.904	5	7	1	2.13	0.27057
+53	I	5	-1	126.904	5	7	1	1.33	0.0804
+53	I	7	-1	126.904	5	7	1	1.33	0.02506
+54	Xe	2	0	131.29	5	8	1	1.3	0.18361
+54	Xe	4	0	131.29	5	8	1	1.3	0.16081
+54	Xe	6	0	131.29	5	8	1	1.3	0.07147
+55	Cs	1	1	132.905	6	1	1	2.46	0.10383
+56	Ba	2	2	137.327	6	2	1	2.01	0.07324
+57	La	3	3	138.906	6	0	3	1.81	0.065
+58	Ce	3	4	140.116	6	0	3	1.71	0.12076
+58	Ce	4	4	140.116	6	0	3	1.71	0.06946
+59	Pr	3	3	140.908	6	0	3	1.71	0.11521
+60	Nd	3	3	144.24	6	0	3	1.71	0.10902
+62	Sm	3	3	150.36	6	0	3	1.71	0.11154
+63	Eu	2	3	151.964	6	0	3	1.71	0.1463
+63	Eu	3	3	151.964	6	0	3	1.71	0.11245
+64	Gd	3	3	157.25	6	0	3	1.66	0.08538
+65	Tb	3	3	158.9254	6	0	3	1.61	0.11187
+65	Tb	4	3	158.9254	6	0	3	1.61	0.99999
+66	Dy	3	3	162.5	6	0	3	1.61	0.1078
+67	Ho	3	3	164.9303	6	0	3	1.61	0.10178
+68	Er	3	3	167.259	6	0	3	1.61	0.10019
+69	Tm	3	3	168.9342	6	0	3	1.61	0.10516
+70	Yb	2	3	173.0545	6	0	3	1.61	0.15535
+70	Yb	3	3	173.0545	6	0	3	1.61	0.10805
+71	Lu	3	3	174.967	6	3	2	1.61	0.0822
+72	Hf	4	4	178.49	6	4	2	1.41	0.05
+73	Ta	2	5	180.949	6	5	2	1.31	0.32162
+73	Ta	3	5	180.949	6	5	2	1.31	0.17543
+73	Ta	4	5	112.411	6	5	2	1.31	0.17543
+73	Ta	5	5	180.948	6	5	2	1.31	0.04545
+74	W	2	6	183.84	6	6	2	1.21	0.32154
+74	W	3	6	183.84	6	6	2	1.21	0.17544
+74	W	4	6	183.84	6	6	2	1.21	0.1608
+74	W	5	6	183.84	6	6	2	1.21	0.14843
+74	W	6	6	183.84	6	6	2	1.21	0.03846
+75	Re	3	7	186.207	6	7	2	1.21	0.17077
+75	Re	4	7	186.207	6	7	2	1.21	0.15315
+75	Re	5	7	186.207	6	7	2	1.21	0.13784
+75	Re	6	7	186.207	6	7	2	1.21	0.14844
+75	Re	7	7	186.207	6	7	2	1.21	0.03333
+76	Os	4	8	190.23	6	8	2	1.16	0.14844
+76	Os	5	8	190.23	6	8	2	1.16	0.13784
+76	Os	6	8	190.23	6	8	2	1.16	0.12865
+76	Os	7	8	190.23	6	8	2	1.16	0.13784
+76	Os	8	8	190.23	6	8	2	1.16	0.0303
+77	Ir	3	5	192.217	6	8	2	1.21	0.16081
+77	Ir	4	5	192.217	6	8	2	1.21	0.11351
+77	Ir	5	5	192.217	6	8	2	1.21	0.13784
+78	Pt	2	2	195.078	6	8	2	1.21	0.19125
+78	Pt	3	2	195.078	6	8	2	1.21	0.17543
+78	Pt	4	2	195.078	6	8	2	1.21	0.13784
+78	Pt	5	2	195.078	6	8	2	1.21	0.10156
+79	Au	1	3	196.967	6	1	2	1.21	0.17705
+79	Au	3	3	196.967	6	1	2	1.21	0.14844
+80	Hg	1	2	200.59	6	2	2	1.36	0.24034
+80	Hg	2	2	200.59	6	2	2	1.36	0.12951
+81	Tl	1	3	204.383	6	3	1	1.76	0.13967
+81	Tl	3	3	204.383	6	3	1	1.76	0.09582
+82	Pb	2	4	207.2	6	4	1	1.66	0.11831
+82	Pb	4	4	207.2	6	4	1	1.66	0.07547
+83	Bi	3	5	208.98	6	5	1	1.46	0.10135
+83	Bi	5	5	208.98	6	5	1	1.46	0.06185
+90	Th	4	4	232.04	7	0	3	1.66	0.069
+92	U	6	6	238.03	7	0	3	1.61	0.03
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/temp.py` & `pybw-23.6.26/pybw/ccnb_mod/bvseLi/temp.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-        
-        
-        
-        
-        bvs.Rmin_moveion = Rmin_moveion
-        
-        if len(bvs._Struct._OxidationTable) == 0:
-            raise Exception('can not calculate BV and Ea without atom oxi info')
-        
-        bvs.stop = False
-        
-        centrepos = np.zeros(bvs._Size + [3])
-        bvs.__Data['BVS'] = np.zeros(bvs._Size, dtype=np.double)
-        bvs.__Data['BVSE'] = np.zeros(bvs._Size, dtype=np.double)
-        bvs.__Data['BVEL'] = np.zeros(bvs._Size, dtype=np.double)
-        
-        for k in range(bvs._Size[2]):
-            for j in range(bvs._Size[1]):
-                for i in range(bvs._Size[0]):
-                    centrepos[i][j][k][2] = k / (bvs._Size[2] - 1.0)
-                    centrepos[i][j][k][1] = j / (bvs._Size[1] - 1.0)
-                    centrepos[i][j][k][0] = i / (bvs._Size[0] - 1.0)
-        
-        if ProgressCall:
-            ProgressCall(0)
-        
-        bvs._poss = bvs._Struct.FracPosToCartPos(centrepos)
-
-        atomsq = {}
-        for atom in bvs._Struct._atomsymbols:
-            atomsq[atom] = 0
-            for site in bvs._Struct._Sites:
-                if atom in site.GetElements():
-                    key = atom + str(site.GetElementsOxiValue()[atom])
-                    atomsq[atom] = atomsq[atom] + site.GetElementsOxiValue()[atom] * site.GetElementsOccupy()[atom] / math.sqrt(bvs._Elementsparam[key][3])
-        
-        qsumanion = 0
-        qsumcation = 0
-        for (atom, value) in atomsq.items():
-            if value > 0:
-                qsumcation = qsumcation + value
-            elif value < 0:
-                qsumanion = qsumanion + value
-            else:
-                qsumanion = 0
-                qsumcation = 0
-        
-        qsum = 0.0
-        if bvs.ValenceOfMoveIon > 0:
-            qsum = -qsumanion / qsumcation
-        else:
-            qsum = -qsumcation / qsumanion
-        
-        key1 = bvs._MoveIon + str(bvs.ValenceOfMoveIon)
-        qm1 = bvs.ValenceOfMoveIon / math.sqrt(bvs._Elementsparam[key1][3])
-        rm1 = bvs._Elementsparam[key1][6]
-        
-        for i in tqdm(range(bvs._Size[0])):
-            (distance, neighborsindex) = bvs._Struct.GetKNeighbors(bvs._poss[i], kn=128)
-            
-            if ProgressCall:
-                ProgressCall(10 + i * 90 / (bvs._Size[0] - 1))
-            
-            for j in range(bvs._Size[1]):
-                
-                for k in range(bvs._Size[2]):
-                    if bvs.stop:
-                        return False
-                    
-                    bvsdata = 0.0
-                    data = 0.0
-                    cdata = 0.0
-                    bvelcdata = 0.0
-                    N = 0
-                    D0 = 0.0
-                    Rcutoff = 10.0
-                    alpha = 0.0
-                    occupyvalue = 0.0
-                    
-                    for dindex, index in enumerate(neighborsindex[j][k]):
-                        site2 = bvs._Struct._SuperCellusites[index]
-                        
-                        if site2.GetIronType() * bvs.ValenceOfMoveIon < 0:
-                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
-                                if ssymbol != 'Vac':
-                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
-                                    if bvs.ValenceOfMoveIon > 0:
-                                        key = "".join([bvs._MoveIon, str(bvs.ValenceOfMoveIon), ssymbol, str(site2oxi)])
-                                    else:
-                                        key = "".join([ssymbol, str(site2oxi), bvs._MoveIon, str(bvs.ValenceOfMoveIon)])
-                                    if (key in bvs._BVSEparam) and (key in bvs._BVparam):
-                                        (Nc, r0, Rcutoff, D0, Rmin, alpha) = bvs._BVSEparam[key][0]
-                                        (r, b) = bvs._BVparam[key][0]
-                                        Rcutoff = 10.0
-                                        if distance[j][k][dindex] <= Rcutoff:
-                                            # bv=np.exp((r0-distance[k][j][i][dindex])*alpha)
-                                            _bvs = np.exp((r - distance[j][k][dindex]) / b)
-                                            smin = np.exp((Rmin - distance[j][k][dindex]) * alpha)
-                                            en_s = np.exp((Rmin - Rcutoff) * alpha)
-                                            bvsdata = bvsdata + _bvs  #*occupyvalue-((en_s-1)**2-1)
-                                            data = data + ((smin - 1)**2 - 1) * occupyvalue
-                                    else:
-                                        if (key not in bvs._BVSEparam):
-                                            raise Exception("bvse {0}  param can't find!!!!".format(key))
-                                            ProgressCall(0)
-                                        else:
-                                            raise Exception("_bvs {0} param can't find!!!!".format(key))
-                                            ProgressCall(0)
-                        else:
-                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
-                                if ssymbol != 'Vac':
-                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
-                                    
-                                    if ssymbol != bvs._MoveIon:
-                                        key = ssymbol + str(site2oxi)
-                                        rm2 = bvs._Elementsparam[key][6]
-                                        qm2 = site2oxi / math.sqrt(bvs._Elementsparam[key][3])
-                                        rm1m2 = distance[j][k][dindex]
-                                        f = 0.74
-                                        if rm1m2 > rm2:
-                                            if rm1m2 < Rcutoff:
-                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
-                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
-                                        else:
-                                            cdata = 300
-                                            bvelcdata = 300
-                                    
-                                    elif ssymbol == bvs._MoveIon:
-                                        key = ssymbol + str(site2oxi)
-                                        rm2 = bvs._Elementsparam[key][6]
-                                        qm2 = site2oxi / math.sqrt(bvs._Elementsparam[key][3])
-                                        rm1m2 = distance[j][k][dindex]
-                                        f = 0.74
-                                        
-                                        if rm1m2 > bvs.Rmin_moveion:
-                                            if rm1m2 < Rcutoff:
-                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
-                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
-                                        else:
-                                            cdata = cdata + 0
+        
+        
+        
+        
+        bvs.Rmin_moveion = Rmin_moveion
+        
+        if len(bvs._Struct._OxidationTable) == 0:
+            raise Exception('can not calculate BV and Ea without atom oxi info')
+        
+        bvs.stop = False
+        
+        centrepos = np.zeros(bvs._Size + [3])
+        bvs.__Data['BVS'] = np.zeros(bvs._Size, dtype=np.double)
+        bvs.__Data['BVSE'] = np.zeros(bvs._Size, dtype=np.double)
+        bvs.__Data['BVEL'] = np.zeros(bvs._Size, dtype=np.double)
+        
+        for k in range(bvs._Size[2]):
+            for j in range(bvs._Size[1]):
+                for i in range(bvs._Size[0]):
+                    centrepos[i][j][k][2] = k / (bvs._Size[2] - 1.0)
+                    centrepos[i][j][k][1] = j / (bvs._Size[1] - 1.0)
+                    centrepos[i][j][k][0] = i / (bvs._Size[0] - 1.0)
+        
+        if ProgressCall:
+            ProgressCall(0)
+        
+        bvs._poss = bvs._Struct.FracPosToCartPos(centrepos)
+
+        atomsq = {}
+        for atom in bvs._Struct._atomsymbols:
+            atomsq[atom] = 0
+            for site in bvs._Struct._Sites:
+                if atom in site.GetElements():
+                    key = atom + str(site.GetElementsOxiValue()[atom])
+                    atomsq[atom] = atomsq[atom] + site.GetElementsOxiValue()[atom] * site.GetElementsOccupy()[atom] / math.sqrt(bvs._Elementsparam[key][3])
+        
+        qsumanion = 0
+        qsumcation = 0
+        for (atom, value) in atomsq.items():
+            if value > 0:
+                qsumcation = qsumcation + value
+            elif value < 0:
+                qsumanion = qsumanion + value
+            else:
+                qsumanion = 0
+                qsumcation = 0
+        
+        qsum = 0.0
+        if bvs.ValenceOfMoveIon > 0:
+            qsum = -qsumanion / qsumcation
+        else:
+            qsum = -qsumcation / qsumanion
+        
+        key1 = bvs._MoveIon + str(bvs.ValenceOfMoveIon)
+        qm1 = bvs.ValenceOfMoveIon / math.sqrt(bvs._Elementsparam[key1][3])
+        rm1 = bvs._Elementsparam[key1][6]
+        
+        for i in tqdm(range(bvs._Size[0])):
+            (distance, neighborsindex) = bvs._Struct.GetKNeighbors(bvs._poss[i], kn=128)
+            
+            if ProgressCall:
+                ProgressCall(10 + i * 90 / (bvs._Size[0] - 1))
+            
+            for j in range(bvs._Size[1]):
+                
+                for k in range(bvs._Size[2]):
+                    if bvs.stop:
+                        return False
+                    
+                    bvsdata = 0.0
+                    data = 0.0
+                    cdata = 0.0
+                    bvelcdata = 0.0
+                    N = 0
+                    D0 = 0.0
+                    Rcutoff = 10.0
+                    alpha = 0.0
+                    occupyvalue = 0.0
+                    
+                    for dindex, index in enumerate(neighborsindex[j][k]):
+                        site2 = bvs._Struct._SuperCellusites[index]
+                        
+                        if site2.GetIronType() * bvs.ValenceOfMoveIon < 0:
+                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
+                                if ssymbol != 'Vac':
+                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
+                                    if bvs.ValenceOfMoveIon > 0:
+                                        key = "".join([bvs._MoveIon, str(bvs.ValenceOfMoveIon), ssymbol, str(site2oxi)])
+                                    else:
+                                        key = "".join([ssymbol, str(site2oxi), bvs._MoveIon, str(bvs.ValenceOfMoveIon)])
+                                    if (key in bvs._BVSEparam) and (key in bvs._BVparam):
+                                        (Nc, r0, Rcutoff, D0, Rmin, alpha) = bvs._BVSEparam[key][0]
+                                        (r, b) = bvs._BVparam[key][0]
+                                        Rcutoff = 10.0
+                                        if distance[j][k][dindex] <= Rcutoff:
+                                            # bv=np.exp((r0-distance[k][j][i][dindex])*alpha)
+                                            _bvs = np.exp((r - distance[j][k][dindex]) / b)
+                                            smin = np.exp((Rmin - distance[j][k][dindex]) * alpha)
+                                            en_s = np.exp((Rmin - Rcutoff) * alpha)
+                                            bvsdata = bvsdata + _bvs  #*occupyvalue-((en_s-1)**2-1)
+                                            data = data + ((smin - 1)**2 - 1) * occupyvalue
+                                    else:
+                                        if (key not in bvs._BVSEparam):
+                                            raise Exception("bvse {0}  param can't find!!!!".format(key))
+                                            ProgressCall(0)
+                                        else:
+                                            raise Exception("_bvs {0} param can't find!!!!".format(key))
+                                            ProgressCall(0)
+                        else:
+                            for (ssymbol, occupyvalue) in site2.GetElementsOccupy().items():
+                                if ssymbol != 'Vac':
+                                    site2oxi = site2.GetElementsOxiValue()[ssymbol]
+                                    
+                                    if ssymbol != bvs._MoveIon:
+                                        key = ssymbol + str(site2oxi)
+                                        rm2 = bvs._Elementsparam[key][6]
+                                        qm2 = site2oxi / math.sqrt(bvs._Elementsparam[key][3])
+                                        rm1m2 = distance[j][k][dindex]
+                                        f = 0.74
+                                        if rm1m2 > rm2:
+                                            if rm1m2 < Rcutoff:
+                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
+                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
+                                        else:
+                                            cdata = 300
+                                            bvelcdata = 300
+                                    
+                                    elif ssymbol == bvs._MoveIon:
+                                        key = ssymbol + str(site2oxi)
+                                        rm2 = bvs._Elementsparam[key][6]
+                                        qm2 = site2oxi / math.sqrt(bvs._Elementsparam[key][3])
+                                        rm1m2 = distance[j][k][dindex]
+                                        f = 0.74
+                                        
+                                        if rm1m2 > bvs.Rmin_moveion:
+                                            if rm1m2 < Rcutoff:
+                                                cdata = cdata + occupyvalue * qm1 * qm2 / rm1m2 * erfc(rm1m2 / (f * (rm1 + rm2))) * qsum
+                                                bvelcdata = bvelcdata + occupyvalue * qm1 * qm2 / rm1m2 * (erfc(rm1m2 / (f * (rm1 + rm2))) - erfc(Rcutoff / (f * (rm1 + rm2))))
+                                        else:
+                                            cdata = cdata + 0
                                             bvelcdata = bvelcdata + 0
```

### Comparing `pybw-23.4.4.2/pybw/ccnb_mod/ccnb_mod.py` & `pybw-23.6.26/pybw/ccnb_mod/ccnb_mod.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw/core/__init__.py` & `pybw-23.6.26/pybw/core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 author: Bowei Pu at 2023.03.01
-version: 2023.03.14
+version: 2023.06.26
 function: Some useful tools
 """
 
 from pybw.tricks.lazy_import import *
 
 
 __author__ = 'Bowei Pu'
-__version__ = '2023.03.11'
+__version__ = '2023.06.26'
 __maintainer__ = 'Bowei Pu'
 __email__ = 'pubowei@foxmail.com'
 __status__ = 'Beta'
-__date__ = '2023-03-11'
+__date__ = '2023-06-26'
 
 
 def time_parser(sec):
     s = int(sec)
     m, sec = s // 60, s % 60
     h, mins = m // 60, m % 60
     day, hour = h // 24, h % 24
@@ -25,19 +25,19 @@
 
 
 def getsizeof(obj):
     return sys.getsizeof(pickle.dumps(obj))
 
 
 class EasyPickle():
-    '''
-    Easy usage for pickle
-    '''
+    """
+    Easy use of pickle
+    """
     def __init__(self):
-        self._function = 'Easy usage for pickle'
+        self._function = 'Easy use of pickle'
     
     @classmethod
     def dump(cls, obj, file_obj):
         pickle.dump(obj, file_obj)
     
     @classmethod
     def load(cls, file_obj):
@@ -58,52 +58,65 @@
 
 class easypickle(EasyPickle):
     def __init__():
         EasyPickle.__init__(self)
 
 
 class PickleDump(EasyPickle):
-    '''
+    """
     Compatible to old version programs
-    '''
+    """
     def __init__():
         EasyPickle.__init__(self)
 
 
 class DictDoc():
-    '''
+    """
     Pack dict to class for easy use
-    '''
+    """
     def __init__(self, dic: dict={}):
-        self.dic = dic
+        self._dic = dic
         self._generate_attributes()
     
     def __repr__(self):
         return '<DictDoc>'
     
     def __str__(self):
         return self.__repr__()
-        
+    
+    def _generate_attributes(self):
+        """
+        Only used when first time load dic
+        """
+        for k, v in self._dic.items():
+            setattr(self, k, v)
+    
+    @property
     def dict(self):
-        return self.dic
+        """
+        Generate vars dict up-to-date
+        """
+        new_dic = vars(self).copy()
+        _ = new_dic.pop('_dic')
+        return new_dic
     
     def as_dict(self):
-        return self.dic
+        return self.dict
     
     def keys(self):
-        return self.dic.keys()
+        return self.dict.keys()
     
     def values(self):
-        return self.dic.values()
-    
-    def _generate_attributes(self):
-        for k, v in self.dic.items():
-            setattr(self, k, v)
+        return self.dict.values()
     
     def setattr(self, name, value):
-        self.dic[name] = value
         setattr(self, name, value)
     
     def add(self, name, value):
         self.setattr(name, value)
     
-    
+
+
+
+
+
+
```

### Comparing `pybw-23.4.4.2/pybw/tricks/lazy_import.py` & `pybw-23.6.26/pybw/tricks/lazy_import.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # function: lazy import
 
 
 ## ------ System ------
 import os
 import sys
 import gc
+import copy
 import shutil
 import time
 # from datetime import datetime
 from glob import glob
 from pathlib import Path
 
 
@@ -20,24 +21,27 @@
 # from func_timeout import func_set_timeout, func_timeout
 
 
 ## ------ Data Analysis ------
 import re
 import random
 import numpy as np
-import pandas as pd
+try:
+    import pandas as pd
+except:
+    pass
 try:
     import polars as pl
 except:
     pass
 
 import matplotlib.pyplot as plt
-plt.rcParams['font.family'] = ['sans-serif']
-plt.rcParams['font.sans-serif'] = ['SimHei']
-plt.rcParams['axes.unicode_minus'] = False
+# plt.rcParams['font.family'] = ['sans-serif']
+# plt.rcParams['font.sans-serif'] = ['SimHei']
+# plt.rcParams['axes.unicode_minus'] = False
 plt.ion()
 # import scienceplots
 plt.style.use('ggplot')
 
 import seaborn as sns
 
 ## ------ Scientific Calculation ------
```

### Comparing `pybw-23.4.4.2/pybw/utils/pymatgen/__init__.py` & `pybw-23.6.26/pybw/utils/pymatgen/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.2/pybw.egg-info/PKG-INFO` & `pybw-23.6.26/pybw.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: pybw
-Version: 23.4.4.2
+Version: 23.6.26
 Summary: pybw
 Home-page: https://gitee.com/pubowei/pybw
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/pybw
 Project-URL: Package, https://pypi.org/project/pybw
 Project-URL: Repo, https://gitee.com/pubowei/pybw
 Keywords: pybw,tools
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pybw
 
 Some convenient useful tools
 
+
+
```

### Comparing `pybw-23.4.4.2/pybw.egg-info/SOURCES.txt` & `pybw-23.6.26/pybw.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 pybw/ccnb_mod/bvseLi/elements.dat
 pybw/ccnb_mod/bvseLi/temp.py
 pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
 pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
 pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
 pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
 pybw/core/__init__.py
+pybw/scholar/__init__.py
 pybw/tricks/__init__.py
 pybw/tricks/lazy_import.py
 pybw/utils/pymatgen/__init__.py
```

### Comparing `pybw-23.4.4.2/setup.py` & `pybw-23.6.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name='pybw',
-    version='23.4.4.2',
+    version='23.6.26',
     python_requires='>=3.6',
     
     author='Bowei Pu',
     author_email='pubowei@foxmail.com',
     
     description='pybw',
     long_description=readme, 
@@ -36,14 +36,15 @@
 
     project_urls={
         'Docs': 'https://gitee.com/pubowei/pybw',
         'Package': 'https://pypi.org/project/pybw',
         'Repo': 'https://gitee.com/pubowei/pybw',
     },
 
+
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.6',
     ],
```

