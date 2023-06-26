# Comparing `tmp/psalpsdtools-0.4.tar.gz` & `tmp/psalpsdtools-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psalpsdtools-0.4.tar", last modified: Mon Jun 26 08:57:21 2023, max compression
+gzip compressed data, was "psalpsdtools-0.5.tar", last modified: Mon Jun 26 09:28:36 2023, max compression
```

## Comparing `psalpsdtools-0.4.tar` & `psalpsdtools-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:57:21.304072 psalpsdtools-0.4/
--rw-rw-rw-   0        0        0      133 2023-06-26 08:57:21.304072 psalpsdtools-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 08:57:21.304072 psalpsdtools-0.4/psalpsdtools/
--rw-rw-rw-   0        0        0     6988 2023-06-26 08:51:15.000000 psalpsdtools-0.4/psalpsdtools/Edrw.py
--rw-rw-rw-   0        0        0     3561 2023-06-26 07:42:15.000000 psalpsdtools-0.4/psalpsdtools/PhRegPrv.py
--rw-rw-rw-   0        0        0       54 2023-06-26 08:56:22.000000 psalpsdtools-0.4/psalpsdtools/__init__.py
--rw-rw-rw-   0        0        0      335 2023-06-26 08:48:08.000000 psalpsdtools-0.4/psalpsdtools/usage.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:57:21.304072 psalpsdtools-0.4/psalpsdtools.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 08:57:21.320858 psalpsdtools-0.4/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-06-26 08:53:21.000000 psalpsdtools-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:28:36.860101 psalpsdtools-0.5/
+-rw-rw-rw-   0        0        0      118 2023-06-26 09:28:36.860101 psalpsdtools-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 09:28:36.844580 psalpsdtools-0.5/psalpsdtools/
+-rw-rw-rw-   0        0        0     6990 2023-06-26 09:25:25.000000 psalpsdtools-0.5/psalpsdtools/Edrw.py
+-rw-rw-rw-   0        0        0     3561 2023-06-26 09:28:20.000000 psalpsdtools-0.5/psalpsdtools/PhRegPrv.py
+-rw-rw-rw-   0        0        0       54 2023-06-26 08:56:22.000000 psalpsdtools-0.5/psalpsdtools/__init__.py
+-rw-rw-rw-   0        0        0      343 2023-06-26 09:28:12.000000 psalpsdtools-0.5/psalpsdtools/usage.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:28:36.860101 psalpsdtools-0.5/psalpsdtools.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-26 09:28:36.000000 psalpsdtools-0.5/psalpsdtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:28:36.860101 psalpsdtools-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-06-26 09:27:56.000000 psalpsdtools-0.5/setup.py
```

### Comparing `psalpsdtools-0.4/psalpsdtools/Edrw.py` & `psalpsdtools-0.5/psalpsdtools/Edrw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from PhRegPrv import PhRegPrv
+from .PhRegPrv import PhRegPrv
 from openpyxl import load_workbook
 import os
-import xlrd
+#import xlrd
 class Edrw:
     def __init__(self):
         pass
     def update_sources(self, regName, qtr, baseFolder, sdFile):
         philippines = PhRegPrv()
         selected_provinces = philippines.get_provinces(regName)
         src = load_workbook(filename = baseFolder + "/" + sdFile, data_only=True)
```

### Comparing `psalpsdtools-0.4/psalpsdtools/PhRegPrv.py` & `psalpsdtools-0.5/psalpsdtools/PhRegPrv.py`

 * *Files identical despite different names*

