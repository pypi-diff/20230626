# Comparing `tmp/psalpsdtools-0.3.tar.gz` & `tmp/psalpsdtools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psalpsdtools-0.3.tar", last modified: Sat Jun 24 13:26:36 2023, max compression
+gzip compressed data, was "psalpsdtools-0.4.tar", last modified: Mon Jun 26 08:57:21 2023, max compression
```

## Comparing `psalpsdtools-0.3.tar` & `psalpsdtools-0.4.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:26:36.011732 psalpsdtools-0.3/
--rw-rw-rw-   0        0        0      229 2023-06-24 13:26:36.011732 psalpsdtools-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 13:26:36.006177 psalpsdtools-0.3/psalpsdtools/
--rw-rw-rw-   0        0        0     4648 2018-06-19 23:16:08.000000 psalpsdtools-0.3/psalpsdtools/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3631 2018-06-19 23:16:08.000000 psalpsdtools-0.3/psalpsdtools/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      932 2018-06-19 23:16:08.000000 psalpsdtools-0.3/psalpsdtools/Generaldistribution.py
--rw-rw-rw-   0        0        0     3550 2023-06-24 12:37:30.000000 psalpsdtools-0.3/psalpsdtools/PhilippinesRegions.py
--rw-rw-rw-   0        0        0     2258 2023-06-22 11:00:11.000000 psalpsdtools-0.3/psalpsdtools/ProvincesOfRegions.py
--rw-rw-rw-   0        0        0      176 2023-06-24 13:09:33.000000 psalpsdtools-0.3/psalpsdtools/__init__.py
--rw-rw-rw-   0        0        0      529 2023-06-24 12:19:00.000000 psalpsdtools-0.3/psalpsdtools/test.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:26:36.010726 psalpsdtools-0.3/psalpsdtools.egg-info/
--rw-rw-rw-   0        0        0      229 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 13:26:36.012731 psalpsdtools-0.3/setup.cfg
--rw-rw-rw-   0        0        0      227 2023-06-24 13:26:12.000000 psalpsdtools-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:57:21.304072 psalpsdtools-0.4/
+-rw-rw-rw-   0        0        0      133 2023-06-26 08:57:21.304072 psalpsdtools-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 08:57:21.304072 psalpsdtools-0.4/psalpsdtools/
+-rw-rw-rw-   0        0        0     6988 2023-06-26 08:51:15.000000 psalpsdtools-0.4/psalpsdtools/Edrw.py
+-rw-rw-rw-   0        0        0     3561 2023-06-26 07:42:15.000000 psalpsdtools-0.4/psalpsdtools/PhRegPrv.py
+-rw-rw-rw-   0        0        0       54 2023-06-26 08:56:22.000000 psalpsdtools-0.4/psalpsdtools/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-06-26 08:48:08.000000 psalpsdtools-0.4/psalpsdtools/usage.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:57:21.304072 psalpsdtools-0.4/psalpsdtools.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-26 08:57:21.000000 psalpsdtools-0.4/psalpsdtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:57:21.320858 psalpsdtools-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-06-26 08:53:21.000000 psalpsdtools-0.4/setup.py
```

### Comparing `psalpsdtools-0.3/psalpsdtools/PhilippinesRegions.py` & `psalpsdtools-0.4/psalpsdtools/PhRegPrv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-class PhilippinesRegions:
+class PhRegPrv:
     def __init__(self):
         self.regions = {
-            "National Capital Region": [
+            "NCR": [
                 "NCR 1",
                 "NCR 2",
                 "NCR 3",
                 "NCR 4",
                 "NCR 5"
             ],
             "Ilocos Region": [
@@ -107,19 +107,20 @@
                 "Surigao del Sur",
             ],
             "BARMM": [
                 "Basilan",
                 "Lanao del Sur",
                 "Maguindanao",
                 "Sulu",
-                "Tawi-Tawi"
+                "Tawi-Tawi",
+                "Eight Area Cluster"
             ]
         }
 
     def get_regions(self):
         return list(self.regions.keys())
 
     def get_provinces(self, region):
         if region in self.regions:
             return self.regions[region]
         else:
-            return []
+            return []
```

