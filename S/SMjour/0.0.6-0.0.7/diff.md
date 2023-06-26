# Comparing `tmp/SMjour-0.0.6.tar.gz` & `tmp/SMjour-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjour-0.0.6.tar", last modified: Mon Jun 12 18:51:32 2023, max compression
+gzip compressed data, was "SMjour-0.0.7.tar", last modified: Mon Jun 26 15:24:04 2023, max compression
```

## Comparing `SMjour-0.0.6.tar` & `SMjour-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:51:32.652000 SMjour-0.0.6/
--rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      448 2023-06-12 18:51:32.640000 SMjour-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:51:32.524000 SMjour-0.0.6/SMjour/
--rw-rw-rw-   0        0        0     6546 2023-06-12 18:50:46.000000 SMjour-0.0.6/SMjour/SMjour.py
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:40.000000 SMjour-0.0.6/SMjour/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:51:32.627000 SMjour-0.0.6/SMjour.egg-info/
--rw-rw-rw-   0        0        0      448 2023-06-12 18:51:32.000000 SMjour-0.0.6/SMjour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-12 18:51:32.000000 SMjour-0.0.6/SMjour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:51:32.000000 SMjour-0.0.6/SMjour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-12 18:51:32.000000 SMjour-0.0.6/SMjour.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 18:51:32.000000 SMjour-0.0.6/SMjour.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      660 2023-06-12 18:51:32.649000 SMjour-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 15:24:04.196000 SMjour-0.0.7/
+-rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-06-26 15:24:04.183000 SMjour-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:24:04.093000 SMjour-0.0.7/SMjour/
+-rw-rw-rw-   0        0        0     6549 2023-06-12 19:29:11.000000 SMjour-0.0.7/SMjour/SMjour.py
+-rw-rw-rw-   0        0        0       13 2023-06-26 15:20:37.000000 SMjour-0.0.7/SMjour/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:24:04.172000 SMjour-0.0.7/SMjour.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-06-26 15:24:03.000000 SMjour-0.0.7/SMjour.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-26 15:24:03.000000 SMjour-0.0.7/SMjour.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:24:03.000000 SMjour-0.0.7/SMjour.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-26 15:24:03.000000 SMjour-0.0.7/SMjour.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 15:24:03.000000 SMjour-0.0.7/SMjour.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      660 2023-06-26 15:24:04.194000 SMjour-0.0.7/setup.cfg
```

### Comparing `SMjour-0.0.6/LICENSE` & `SMjour-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjour-0.0.6/SMjour/SMjour.py` & `SMjour-0.0.7/SMjour/SMjour.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import plotly.express as px
 from google.colab import drive
 
 
-def input_path(message):
+def input_path(message=""):
   raw_s=input(message)
   raw_s=raw_s.replace(r'"','')
   return "/content/drive/Shareddrives/"+'/'.join(raw_s.split("\\")[2:])
    
 def get_data():
     #import drive
     drive.mount("/content/drive")
```

### Comparing `SMjour-0.0.6/setup.cfg` & `SMjour-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 4d6a 6f75 720d 0a76 6572 7369   = SMjour..versi
-00000020: 6f6e 203d 2030 2e30 2e36 0d0a 6175 7468  on = 0.0.6..auth
+00000020: 6f6e 203d 2030 2e30 2e37 0d0a 6175 7468  on = 0.0.7..auth
 00000030: 6f72 203d 2041 6775 7374 696e 2042 7573  or = Agustin Bus
 00000040: 746f 7320 4261 7274 6f6e 0d0a 6175 7468  tos Barton..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6775 7374  or_email = agust
 00000060: 696e 6275 7374 6f73 6261 7274 6f6e 4067  inbustosbarton@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 696e 7665 7374 6967  ption = investig
 00000090: 6174 696f 6e20 6a6f 7572 6e61 6c0d 0a6c  ation journal..l
```

