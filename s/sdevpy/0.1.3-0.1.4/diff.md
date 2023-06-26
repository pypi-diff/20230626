# Comparing `tmp/sdevpy-0.1.3.tar.gz` & `tmp/sdevpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.1.3.tar", last modified: Thu Jun 22 05:04:48 2023, max compression
+gzip compressed data, was "sdevpy-0.1.4.tar", last modified: Mon Jun 26 07:50:15 2023, max compression
```

## Comparing `sdevpy-0.1.3.tar` & `sdevpy-0.1.4.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.200909 sdevpy-0.1.3/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1725 2023-06-22 05:04:48.197910 sdevpy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.1.3/README.md
--rw-rw-rw-   0        0        0      655 2023-06-22 05:01:38.000000 sdevpy-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 05:04:48.200909 sdevpy-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.080948 sdevpy-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.096943 sdevpy-0.1.3/src/sdevpy/
--rw-rw-rw-   0        0        0       23 2023-06-19 11:53:52.000000 sdevpy-0.1.3/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.141928 sdevpy-0.1.3/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.1.3/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.1.3/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6308 2023-06-20 03:41:05.000000 sdevpy-0.1.3/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6911 2023-06-20 03:42:55.000000 sdevpy-0.1.3/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.1.3/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8745 2023-06-20 03:49:45.000000 sdevpy-0.1.3/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.1.3/src/sdevpy/analytics/sabr.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.150925 sdevpy-0.1.3/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.1.3/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.1.3/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.1.3/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.1.3/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.1.3/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.158923 sdevpy-0.1.3/src/sdevpy/maths/
--rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.1.3/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      413 2023-06-20 08:24:06.000000 sdevpy-0.1.3/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.1.3/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.1.3/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.160922 sdevpy-0.1.3/src/sdevpy/projects/
--rw-rw-rw-   0        0        0      893 2023-06-19 11:54:24.000000 sdevpy-0.1.3/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.164921 sdevpy-0.1.3/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.1.3/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.1.3/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.1.3/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.172918 sdevpy-0.1.3/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0     2513 2023-06-21 13:29:16.000000 sdevpy-0.1.3/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     5033 2023-06-21 13:31:09.000000 sdevpy-0.1.3/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0    10181 2023-06-21 13:31:58.000000 sdevpy-0.1.3/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0    10577 2023-06-21 13:33:49.000000 sdevpy-0.1.3/src/sdevpy/projects/stovol/xsabrfit.py
--rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.1.3/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.1.3/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.184914 sdevpy-0.1.3/src/sdevpy/tools/
--rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.1.3/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.1.3/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1572 2023-06-22 05:01:01.000000 sdevpy-0.1.3/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.1.3/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.1.3/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.1.3/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.195911 sdevpy-0.1.3/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0     2529 2023-06-21 13:34:01.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     8773 2023-06-20 09:22:19.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     9366 2023-06-21 13:33:57.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     9324 2023-06-21 13:23:45.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0    11547 2023-06-21 13:33:58.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     4789 2023-06-21 13:33:59.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     2118 2023-06-21 13:34:03.000000 sdevpy-0.1.3/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.125936 sdevpy-0.1.3/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0     1725 2023-06-22 05:04:48.000000 sdevpy-0.1.3/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2023-06-22 05:04:48.000000 sdevpy-0.1.3/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 05:04:48.000000 sdevpy-0.1.3/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-22 05:04:48.000000 sdevpy-0.1.3/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 05:04:48.000000 sdevpy-0.1.3/src/sdevpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 05:04:48.196910 sdevpy-0.1.3/tests/
--rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.1.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.889090 sdevpy-0.1.4/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1725 2023-06-26 07:50:15.879093 sdevpy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.1.4/README.md
+-rw-rw-rw-   0        0        0      695 2023-06-25 09:23:28.000000 sdevpy-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 07:50:15.890089 sdevpy-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.459229 sdevpy-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.490219 sdevpy-0.1.4/src/sdevpy/
+-rw-rw-rw-   0        0        0       23 2023-06-25 09:21:00.000000 sdevpy-0.1.4/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.597185 sdevpy-0.1.4/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.1.4/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.1.4/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6316 2023-06-22 09:20:26.000000 sdevpy-0.1.4/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6913 2023-06-24 04:26:35.000000 sdevpy-0.1.4/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.1.4/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8745 2023-06-20 03:49:45.000000 sdevpy-0.1.4/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.1.4/src/sdevpy/analytics/sabr.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.633173 sdevpy-0.1.4/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.1.4/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     2504 2023-06-25 06:30:01.000000 sdevpy-0.1.4/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.1.4/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.1.4/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.1.4/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.668161 sdevpy-0.1.4/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.1.4/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      654 2023-06-24 09:12:10.000000 sdevpy-0.1.4/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.1.4/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.1.4/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.676159 sdevpy-0.1.4/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0      893 2023-06-25 05:21:23.000000 sdevpy-0.1.4/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.711147 sdevpy-0.1.4/src/sdevpy/projects/pinns/
+-rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.1.4/src/sdevpy/projects/pinns/ernst_pinns.py
+-rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.1.4/src/sdevpy/projects/pinns/pinns.py
+-rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.1.4/src/sdevpy/projects/pinns/pinns_worst_of.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.745136 sdevpy-0.1.4/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0     3351 2023-06-24 07:11:00.000000 sdevpy-0.1.4/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     5033 2023-06-21 13:31:09.000000 sdevpy-0.1.4/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0    10803 2023-06-26 01:33:23.000000 sdevpy-0.1.4/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.1.4/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     7644 2023-06-26 06:59:16.000000 sdevpy-0.1.4/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.795120 sdevpy-0.1.4/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.1.4/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.1.4/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1759 2023-06-25 09:09:17.000000 sdevpy-0.1.4/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.1.4/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     3426 2023-06-24 04:23:59.000000 sdevpy-0.1.4/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.1.4/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.856100 sdevpy-0.1.4/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0     2377 2023-06-24 06:47:56.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     9160 2023-06-24 06:47:14.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     2534 2023-06-24 06:42:09.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     8564 2023-06-24 06:46:09.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0     9278 2023-06-24 06:37:02.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     5807 2023-06-24 05:59:47.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     1705 2023-06-24 06:53:18.000000 sdevpy-0.1.4/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.538204 sdevpy-0.1.4/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0     1725 2023-06-26 07:50:15.000000 sdevpy-0.1.4/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1591 2023-06-26 07:50:15.000000 sdevpy-0.1.4/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:50:15.000000 sdevpy-0.1.4/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-26 07:50:15.000000 sdevpy-0.1.4/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 07:50:15.000000 sdevpy-0.1.4/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 07:50:15.866097 sdevpy-0.1.4/tests/
+-rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.1.4/tests/test.py
```

### Comparing `sdevpy-0.1.3/LICENSE` & `sdevpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/PKG-INFO` & `sdevpy-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.1.3/README.md` & `sdevpy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/pyproject.toml` & `sdevpy-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-	"pandas","pyperclip","py_vollib"
+	"pandas","pyperclip","py_vollib","numpy","tensorflow",
+  "scikit-learn"
 ]
 
 [project.urls]
 "Git page" = "https://github.com/sebgur/SDev.Python"
 "SDev Finance" = "http://sdev-finance.com/"
```

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.1.4/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/black.py` & `sdevpy-0.1.4/src/sdevpy/analytics/black.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.1.4/src/sdevpy/analytics/fbsabr.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,23 +105,23 @@
     """ Calculate parameter alpha with our definition in terms of ln_vol, i.e.
         alpha = ln_vol * fwd ^ (1.0 - beta) """
     floor = 0.00001
     abs_f = np.maximum(np.abs(fwd), floor)
     return ln_vol * abs_f ** (1.0 - beta)
 
 if __name__ == "__main__":
-    EXPIRIES = [0.05, 0.10, 0.25, 0.5]
+    EXPIRIES = [3.0, 8.0, 13, 19, 22, 31, 34]
     NSTRIKES = 50
-    FWD = -0.005
-    SHIFT = 0.03
+    FWD = 0.016132
+    SHIFT = 0.00
     SFWD = FWD + SHIFT
     IS_CALL = False
     ARE_CALLS = [IS_CALL] * NSTRIKES
     ARE_CALLS = [ARE_CALLS] * len(EXPIRIES)
-    LNVOL = 0.25
+    LNVOL = 0.48
     # Spread method
     # SPREADS = np.linspace(-200, 200, NSTRIKES)
     # SPREADS = np.asarray([SPREADS] * len(EXPIRIES))
     # STRIKES = FWD + SPREADS / 10000.0
     # SSTRIKES = STRIKES + SHIFT
     # XAXIS = SPREADS
     # Distribution method
@@ -130,19 +130,19 @@
     PERCENT = np.asarray([PERCENT] * len(EXPIRIES))
     ITO = -0.5 * LNVOL**2 * np_expiries
     DIFF = LNVOL * np.sqrt(np_expiries) * sp.norm.ppf(PERCENT)
     SSTRIKES = SFWD * np.exp(ITO + DIFF)
     STRIKES = SSTRIKES - SHIFT
     XAXIS = STRIKES
 
-    PARAMETERS = {'LnVol': LNVOL, 'Beta': 0.1, 'Nu': 0.50, 'Rho': -0.25}
+    PARAMETERS = {'LnVol': LNVOL, 'Beta': 0.5, 'Nu': 0.66, 'Rho': 0.48}
     NUM_MC = 100 * 1000
     POINTS_PER_YEAR = 25
-    # SCHEME = 'Andersen'
-    SCHEME = 'Euler'
+    SCHEME = 'Andersen'
+    # SCHEME = 'Euler'
 
     # Calculate MC prices
     mc_timer = timer.Stopwatch("MC")
     mc_timer.trigger()
     MC_PRICES = price(EXPIRIES, STRIKES, ARE_CALLS, FWD, PARAMETERS, NUM_MC, POINTS_PER_YEAR,
                       scheme=SCHEME)
     mc_timer.stop()
```

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.1.4/src/sdevpy/analytics/mcheston.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     # Build time grid
     time_grid_builder = SimpleTimeGridBuilder(points_per_year=points_per_year)
     time_grid_builder.add_grid(expiries)
     time_grid = time_grid_builder.complete_grid()
     num_factors = 2
 
+
     # Find payoff times
     is_payoff = np.in1d(time_grid, expiries)
 
     # Retrieve parameters
     lnvol = parameters['LnVol']
     kappa = parameters['Kappa']
     theta = parameters['Theta']
```

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.1.4/src/sdevpy/analytics/mcsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.1.4/src/sdevpy/analytics/mczabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/analytics/sabr.py` & `sdevpy-0.1.4/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.1.4/src/sdevpy/machinelearning/callbacks.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.1.4/src/sdevpy/machinelearning/learningmodel.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.1.4/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.1.4/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/maths/interpolations.py` & `sdevpy-0.1.4/src/sdevpy/maths/interpolations.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/maths/rand.py` & `sdevpy-0.1.4/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/datafiles.py` & `sdevpy-0.1.4/src/sdevpy/projects/datafiles.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/pinns/ernst_pinns.py` & `sdevpy-0.1.4/src/sdevpy/projects/pinns/ernst_pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/pinns/pinns.py` & `sdevpy-0.1.4/src/sdevpy/projects/pinns/pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/pinns/pinns_worst_of.py` & `sdevpy-0.1.4/src/sdevpy/projects/pinns/pinns_worst_of.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.1.4/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 """ Generate training data for Stochastic Local Vol models. We implement the direct map here.
     Datasets of parameters (inputs) vs prices/implied vols (outputs) are generated to later train
     a network that learns the so-called 'direct' calculation, i.e. prices from parameter. """
 import os
 from sdevpy.volsurfacegen import stovolfactory
 from sdevpy import settings
-from sdevpy.tools.filemanager import check_directory
+from sdevpy.tools import filemanager
 from sdevpy.tools.timer import Stopwatch
 
 
 # ################ Runtime configuration ##########################################################
 # MODEL_TYPE = "SABR"
-# MODEL_TYPE = "ShiftedSABR"
-# MODEL_TYPE = "McShiftedSABR"
-MODEL_TYPE = "FbSABR"
-# MODEL_TYPE = "McShiftedZABR"
-# MODEL_TYPE = "McShiftedHeston"
-NUM_SAMPLES = 400 * 1000
+# MODEL_TYPE = "McSABR"
+# MODEL_TYPE = "FbSABR"
+# MODEL_TYPE = "McZABR"
+MODEL_TYPE = "McHeston"
+SHIFT = 0.03
+NUM_SAMPLES = 1 * 1000
 # The 4 parameters below are only relevant for models whose reference is calculated by MC
 NUM_EXPIRIES = 10
-SURFACE_SIZE = 50
+NUM_STRIKES = 5
 NUM_MC = 100 * 1000 # 100 * 1000
 POINTS_PER_YEAR = 25 # 25
 SEED = 42# [123456789, 6789, 9191, 888, 4321, 100, 4444, 72, 1234, 42]
 
 print(">> Set up runtime configuration")
 project_folder = os.path.join(settings.WORKFOLDER, "stovol")
 print("> Project folder: " + project_folder)
 data_folder = os.path.join(project_folder, "samples")
 print("> Data folder: " + data_folder)
-check_directory(data_folder)
+filemanager.check_directory(data_folder)
 print("> Chosen model: " + MODEL_TYPE)
 data_file = os.path.join(data_folder, MODEL_TYPE + "_samples.tsv")
 
-# ################ Select model ###############################################################
-generator = stovolfactory.set_generator(MODEL_TYPE, NUM_EXPIRIES, SURFACE_SIZE, NUM_MC,
+# ################ Select model ###################################################################
+generator = stovolfactory.set_generator(MODEL_TYPE, SHIFT, NUM_EXPIRIES, NUM_STRIKES, NUM_MC,
                                         POINTS_PER_YEAR, SEED)
 
+# ################ Select training ranges #########################################################
+# # SABR
+# RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.5],
+#           'Beta': [0.1, 0.9], 'Nu': [0.1, 1.0], 'Rho': [-0.6, 0.6]}
+# # ZABR
+# RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.25],
+#           'Beta': [0.49, 0.51], 'Nu': [0.20, 0.80], 'Rho': [-0.4, 0.4],
+#           'Gamma': [0.10, 0.9]}
+# Heston
+RANGES = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041], 'LnVol': [0.05, 0.25],
+          'Kappa': [0.25, 4.00], 'Theta': [0.05**2, 0.25**2], 'Xi': [0.10, 0.50],
+          'Rho': [-0.40, 0.40]}
+
 # ################ Generate dataset ###############################################################
 print(">> Generate dataset")
 
 print(f"> Generate {NUM_SAMPLES:,} price samples")
 timer_gen = Stopwatch("Generating Samples")
 timer_gen.trigger()
-data_df = generator.generate_samples(NUM_SAMPLES)
+data_df = generator.generate_samples(NUM_SAMPLES, RANGES)
+# full_data_file = os.path.join(data_folder, MODEL_TYPE + "_samples_full.tsv")
+# generator.to_file(data_df, full_data_file)
 timer_gen.stop()
 
 print("> Convert to normal vol and cleanse data")
 timer_conv = Stopwatch("Converting Prices")
 timer_conv.trigger()
 data_df = generator.to_nvol(data_df, cleanse=True)
 num_clean = len(data_df.index)
```

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/stovol/stovolplot.py` & `sdevpy-0.1.4/src/sdevpy/projects/stovol/stovolplot.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.1.4/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,96 +9,108 @@
 import tensorflow as tf
 import matplotlib.pyplot as plt
 from sdevpy import settings
 from sdevpy.machinelearning.topology import compose_model
 from sdevpy.machinelearning.learningmodel import LearningModel, load_learning_model
 from sdevpy.machinelearning.learningschedules import FlooredExponentialDecay
 from sdevpy.machinelearning.callbacks import RefCallback
-from sdevpy.machinelearning.datasets import prepare_sets
-from sdevpy.tools.filemanager import check_directory
+from sdevpy.machinelearning import datasets
+from sdevpy.tools import filemanager
 from sdevpy.tools.timer import Stopwatch
 from sdevpy.tools import clipboard
-from sdevpy.maths.metrics import rmse, tf_rmse
+from sdevpy.maths.metrics import bps_rmse, tf_bps_rmse
 from sdevpy.volsurfacegen.stovolfactory import set_generator
 from sdevpy.projects.stovol import stovolplot as xplt
 
+
+# Implement DOWNLOAD_DATASET for TRAIN = True
+# Create Colab to generate, Colab to train
 # Fine-train models
-# Use type in json to know which type to instantiate
-# Lazy instantiation from remote/name code
 # Store data in Kaggle
 
 # ################ Runtime configuration ##########################################################
-# MODEL_TYPE = "SABR"
-# MODEL_TYPE = "ShiftedSABR"
-# MODEL_TYPE = "McShiftedSABR"
-MODEL_TYPE = "FbSABR"
-# MODEL_TYPE = "McShiftedZABR"
-# MODEL_TYPE = "McShiftedHeston"
+MODEL_TYPE = "SABR"
+# MODEL_TYPE = "McSABR"
+# MODEL_TYPE = "FbSABR"
+# MODEL_TYPE = "McZABR"
+# MODEL_TYPE = "McHeston"
+MODEL_ID = "SABR_3L_64n" # Pre-trained model ID (we can pre-train several versions)
+SHIFT = 0.03
 USE_TRAINED = True
+DOWNLOAD_MODELS = True # Only used when USE_TRAINED is True
+DOWNLOAD_DATASETS = True # Use when already created/downloaded
 TRAIN = False
 if USE_TRAINED is False and TRAIN is False:
     raise RuntimeError("When not using pre-trained models, a new model must be trained")
 
+NUM_SAMPLES = 500 * 1000 # Number of samples to read from sample files
 TRAIN_PERCENT = 0.90 # Proportion of dataset used for training (rest used for test)
 EPOCHS = 100
 BATCH_SIZE = 1000
 SHOW_VOL_CHARTS = True # Show smile section charts
 # For comparison to reference values (accuracy of reference)
 NUM_MC = 100 * 1000 # 100 * 1000
 POINTS_PER_YEAR = 25 # 25
 
 print(">> Set up runtime configuration")
+print("> Chosen model type: " + MODEL_TYPE)
+if USE_TRAINED:
+    print("> Pre-trained model ID: " + MODEL_ID)
+
 project_folder = os.path.join(settings.WORKFOLDER, "stovol")
 print("> Project folder: " + project_folder)
-data_folder = os.path.join(project_folder, "samples")
+sample_folder = os.path.join(project_folder, "samples")
+data_folder = os.path.join(sample_folder, MODEL_TYPE)
 print("> Data folder: " + data_folder)
-check_directory(data_folder)
-print("> Chosen model: " + MODEL_TYPE)
-data_file = os.path.join(data_folder, MODEL_TYPE + "_samples.tsv")
+data_file = os.path.join(sample_folder, MODEL_TYPE + "_samples.tsv")
+print("> Data file: " + data_file)
 model_folder = os.path.join(project_folder, "models")
 print("> Model folder: " + model_folder)
 
-# ################ Helper functions ###############################################################
-def bps_rmse(y_true, y_ref):
-    """ RMSE in bps """
-    return 10000.0 * rmse(y_true, y_ref)
-
-def tf_bps_rmse(y_true, y_ref):
-    """ RMSE in bps in tensorflow """
-    return 10000.0 * tf_rmse(y_true, y_ref)
+if USE_TRAINED and DOWNLOAD_MODELS:
+    url = 'https://github.com/sebgur/SDev.Python/raw/main/models/stovol/stovol.zip'
+    print("> Downloading and unzipping models from: " + url)
+    filemanager.download_unzip(url, model_folder)
+
+if DOWNLOAD_DATASETS:
+    print("> Downloading datasets from: ")
 
 # ################ Select generator ###############################################################
 # Select generator. The number of expiries and surface size are irrelevant as here we do not
 # generate sample data but read it from files. Number of MC and points per year are required
 # to calculate the reference values against which we can validate the model.
-generator = set_generator(MODEL_TYPE, num_mc=NUM_MC, points_per_year=POINTS_PER_YEAR)
+generator = set_generator(MODEL_TYPE, shift=SHIFT, num_mc=NUM_MC, points_per_year=POINTS_PER_YEAR)
 
 # ################ Prepare datasets ###############################################################
 # Datasets are always read, as even if we don't train, we're still going to evaluate the
 # performance of the pre-trained model
 print(">> Preparing datasets")
+# Retrieve data from dataset folder
+datasets.retrieve_data(data_folder, NUM_SAMPLES, shuffle=True, export_file=data_file)
 # Retrieve dataset
 print("> Reading dataset from file: " + data_file)
 x_set, y_set, data_df = generator.retrieve_datasets(data_file, shuffle=True)
 input_dim = x_set.shape[1]
 output_dim = y_set.shape[1]
 print("> Input dimension: " + str(input_dim))
 print("> Output dimension: " + str(output_dim))
 print("> Dataset extract")
 print(data_df.head())
 # Split into training and test sets
 TRS = TRAIN_PERCENT * 100
 print(f"> Splitting between training set ({TRS:.2f}%) and test set ({100 - TRS:.2f}%)")
-x_train, y_train, x_test, y_test = prepare_sets(x_set, y_set, TRAIN_PERCENT)
+x_train, y_train, x_test, y_test = datasets.prepare_sets(x_set, y_set, TRAIN_PERCENT)
+print(f"> Training set size: {x_train.shape[0]:,}")
+print(f"> Testing set size: {x_test.shape[0]:,}")
 
 # ################ Compose/Load the model #########################################################
 # Compose new model or load pre-trained one
 if USE_TRAINED:
     print(">> Loading pre-trained model")
-    model_folder_name = os.path.join(model_folder, MODEL_TYPE)
+    model_folder_name = os.path.join(model_folder, MODEL_ID)
     print("> Loading pre-trained model from: " + model_folder_name)
     model = load_learning_model(model_folder_name)
     keras_model = model.model
     HIDDEN_LAYERS = NUM_NEURONS = DROP_OUT = None
     topology = model.topology_
     if topology is not None:
         HIDDEN_LAYERS = topology['layers']
@@ -134,34 +146,27 @@
     optimizer = tf.keras.optimizers.Adam(learning_rate=lr_schedule)
     model.optimizer_ = optimizer.get_config()
     print("> Optimizer settings")
     optim_fields = model.optimizer_
     for field, value in optim_fields.items():
         print("> ", field, ":", value)
 
-
     # Compile
     print("> Compile model")
     keras_model.compile(loss=tf_bps_rmse, optimizer=optimizer)
 
-
     # Callbacks
     EPOCH_SAMPLING = 5
     callback = RefCallback(x_test, y_test, bps_rmse, optimizer=optimizer,
                            epoch_sampling=EPOCH_SAMPLING)
-    # callback = None
-    # callback = SDevPyCallback(optimizer=optimizer, epoch_sampling=EPOCH_SAMPLING)
 
     # Train the network
     print(">> Training ANN model")
     trn_timer = Stopwatch("Training")
     trn_timer.trigger()
-    # shuffled_indices = np.random.permutation(x_train.shape[0])
-    # x_train = x_train[shuffled_indices]
-    # y_train = y_train[shuffled_indices]
     model.train(x_train, y_train, EPOCHS, BATCH_SIZE, callback)
     trn_timer.stop()
     trn_timer.print()
 
     # Save trained model to file
     now = datetime.now()
     dt_string = now.strftime("%Y%m%d-%H_%M_%S")
@@ -173,50 +178,59 @@
 # ################ Performance analysis ###########################################################
 # Analyse results
 print(">> Analyse results")
 
 # Check performance
 train_pred = model.predict(x_train)
 train_rmse = bps_rmse(train_pred, y_train)
-print(f"RMSE(nvol) on training set: {train_rmse:,.2f}")
+print(f"> RMSE(nvol) on training set: {train_rmse:,.2f}")
 
 test_pred = model.predict(x_test)
 test_rmse = bps_rmse(test_pred, y_test)
-print(f"RMSE(nvol) on test set: {test_rmse:,.2f}")
+print(f"> RMSE(nvol) on test set: {test_rmse:,.2f}")
 
 # Generate strike spread axis
 if SHOW_VOL_CHARTS:
+    print("> Choosing a sample parameter set to display chart")
     NUM_STRIKES = 100
     PARAMS = { 'LnVol': 0.20, 'Beta': 0.5, 'Nu': 0.55, 'Rho': -0.25, 'Gamma': 0.7, 'Kappa': 1.0,
                 'Theta': 0.05, 'Xi': 0.50 }
     FWD = 0.028
 
     # Any number of expiries can be calculated, but for optimum display choose no more than 6
-    EXPIRIES = np.asarray([0.125, 0.250, 0.5, 1.00, 2.0, 5.0]).reshape(-1, 1)
-    # EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
+    # EXPIRIES = np.asarray([0.125, 0.250, 0.5, 1.00, 2.0, 5.0]).reshape(-1, 1)
+    EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
     NUM_EXPIRIES = EXPIRIES.shape[0]
     METHOD = 'Percentiles'
     PERCENTS = np.linspace(0.01, 0.99, num=NUM_STRIKES)
     PERCENTS = np.asarray([PERCENTS] * NUM_EXPIRIES)
 
     strikes = generator.convert_strikes(EXPIRIES, PERCENTS, FWD, PARAMS, METHOD)
     clipboard.export2d(strikes)
     ARE_CALLS = [[False] * NUM_STRIKES] * NUM_EXPIRIES # All puts
     # ARE_CALLS = [[False if s < FWD else True for s in expks] for expks in strikes] # Puts/calls
     # print(ARE_CALLS)
 
-    print("Calculating chart surface with reference model")
+    print("> Calculating chart surface with reference model")
+    timer_ref = Stopwatch("Reference surface calculation")
+    timer_ref.trigger()
     ref_prices = generator.price_surface_ref(EXPIRIES, strikes, ARE_CALLS, FWD, PARAMS)
-    # print(ref_prices.shape)
+    timer_ref.stop()
     # clipboard.export2d(ref_prices)
-    print("Calculating chart surface with trained model")
+    print("> Calculating chart surface with trained model")
+    timer_mod = Stopwatch("Model surface calculation")
+    timer_mod.trigger()
     mod_prices = generator.price_surface_mod(model, EXPIRIES, strikes, ARE_CALLS, FWD, PARAMS)
-    # print(mod_prices.shape)
+    timer_mod.stop()
     # clipboard.export2d(mod_prices)
-    print(f"Ref-Mod RMSE(price): {bps_rmse(ref_prices, mod_prices):.2f}")
+    print(f"> Ref-Mod RMSE(price): {bps_rmse(ref_prices, mod_prices):.2f}")
+
+    # Display timers
+    timer_ref.print()
+    timer_mod.print()
 
     # Available tranforms: Price, ShiftedBlackScholes, Bachelier
     TITLE = f"{MODEL_TYPE} smile sections, forward={FWD*100:.2f}"#,%\n parameters={PARAMS}"
     # TRANSFORM = "Bachelier"
     # TRANSFORM = "Price"
     TRANSFORM = "ShiftedBlackScholes"
     xplt.plot_transform_surface(EXPIRIES, strikes, ARE_CALLS, FWD, ref_prices, mod_prices,
```

### Comparing `sdevpy-0.1.3/src/sdevpy/tools/clipboard.py` & `sdevpy-0.1.4/src/sdevpy/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/tools/filemanager.py` & `sdevpy-0.1.4/src/sdevpy/tools/filemanager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 """ File management utilities """
 import os
 import csv
-# import winsound
-import datetime as dt
+# import datetime as dt
 import pathlib
+from io import BytesIO
+import zipfile as zf
+import requests
+
+
+def download_unzip(zip_url, extract_folder, save_file=False):
+    """ Download zip file from url and unzip """
+    req = requests.get(zip_url, timeout=10)
+
+    if save_file:
+        down_filename = zip_url.split('/')[-1]
+        with open(down_filename,'wb') as output_file:
+            output_file.write(req.content)
+
+    with zf.ZipFile(BytesIO(req.content)) as zip_file:
+        zip_file.extractall(extract_folder)
+
+    # zipfile = zf.ZipFile(BytesIO(req.content))
+    # zipfile.extractall(extract_folder)
 
 
 def check_directory(path):
     """ Creates directory if it does not already exist """
     path_exists = os.path.exists(path)
     if not path_exists:
         os.makedirs(path)
@@ -27,33 +45,20 @@
 #     for r, d, f in os.walk(path):
 #         for file in f:
 #             if '.csv' in file:
 #                 files.append(os.path.join(r, file))
 
 #     return files
 
+
 def list_files(path, extensions=None):
     """ List all files in a path that have the extensions """
     all_files = os.listdir(path)
     if extensions is None:
         return all_files
     else:
         files = []
         for f in all_files:
             if pathlib.Path(f).suffix in extensions:
                 files.append(f)
 
         return files
-
-# def make_a_noise(beep=True):
-#     """ Make a noise """
-#     if beep:
-#         f1 = 500
-#         f2 = 1000
-#         duration = 300
-#         winsound.Beep(f1, duration)
-#         winsound.Beep(f2, duration)
-#         winsound.Beep(f1, duration)
-
-#     now = dt.datetime.now()
-#     dt_string = now.strftime("%H:%M:%S, %d/%m/%Y")
-#     print("Closing at ", dt_string)
```

### Comparing `sdevpy-0.1.3/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.1.4/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/tools/timegrids.py` & `sdevpy-0.1.4/src/sdevpy/tools/timegrids.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         for d in dates:
             times.append(model_time(val_date, d))
 
         self.time_grid_.extend(times)
 
     def add_grid(self, times):
         """ Add vector of times """
-        self.time_grid_.extend(times)
+        self.time_grid_.extend(times.reshape(-1))
 
     def refine(self):
         """ Add a fine grid to the current grid """
         self.time_grid_.extend(self.fine_grid())
 
     def clean(self):
         """ Remove negative times and duplicates, then sort in ascending order """
@@ -78,12 +78,28 @@
     base = date(2023, 1, 24)
     fixing = date(2022, 1, 24)
     monitor = date(2024, 1, 24)
     expiry = date(2025, 1, 24)
     settlement = date(2026, 1, 24)
     builder = SimpleTimeGridBuilder(5)
     builder.add_dates(base, [fixing, settlement, expiry, monitor, settlement])
-    print(builder.time_grid_)
+    # print(builder.time_grid_)
     builder.refine()
-    print(builder.time_grid_)
+    # print(builder.time_grid_)
     builder.clean()
-    print(builder.time_grid_)
+    # print(builder.time_grid_)
+
+    # Test MC situation
+    time_grid_builder = SimpleTimeGridBuilder(points_per_year=5)
+    EXPIRIES = np.asarray([5.0, 1.0, 0.125, 0.250, 0.5]).reshape(-1, 1)
+    print(EXPIRIES)
+    time_grid_builder.add_grid(EXPIRIES)
+    print(time_grid_builder.time_grid_)
+    print("refine")
+    time_grid_builder.refine()
+    print(time_grid_builder.time_grid_)
+    print("clean")
+    time_grid_builder.clean()
+    tg = time_grid_builder.time_grid_
+    print(tg)
+    # time_grid = time_grid_builder.complete_grid()
+
```

### Comparing `sdevpy-0.1.3/src/sdevpy/tools/timer.py` & `sdevpy-0.1.4/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.3/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.1.4/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,80 +2,75 @@
 import os
 import numpy as np
 import pandas as pd
 import scipy.stats as sp
 from sdevpy import settings
 from sdevpy.analytics import mcheston
 from sdevpy.analytics import bachelier
-from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator
 from sdevpy.volsurfacegen.smilegenerator import SmileGenerator
 from sdevpy.tools import filemanager
 from sdevpy.tools import timer
 
 
-class McHestonGenerator(SabrGenerator):
+class McHestonGenerator(SmileGenerator):
     """ Heston model with a generic shift value, using Monte-Carlo to calculate option prices. """
     def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, num_mc=10000,
-                 points_per_year=10):
-        SabrGenerator.__init__(self, shift)
-        self.num_strikes = num_strikes
-        self.num_expiries = num_expiries
-        self.surface_size = self.num_expiries * self.num_strikes
+                 points_per_year=10, seed=42):
+        SmileGenerator.__init__(self, shift, num_expiries, num_strikes, seed=seed)
         self.num_mc = num_mc
         self.points_per_year = points_per_year
-        self.are_calls = [[self.is_call] * self.num_strikes] * self.num_expiries
 
-    def generate_samples(self, num_samples):
+    def generate_samples(self, num_samples, rg):
         shift = self.shift
 
         print(f"Number of strikes: {self.num_strikes:,}")
         print(f"Number of expiries: {self.num_expiries:,}")
         print(f"Surface size: {self.surface_size:,}")
         print(f"Number of samples: {num_samples:,}")
 
         # Derive number of surfaces to generate
         num_surfaces = int(num_samples / self.surface_size)# + 1)
         print(f"Number of surfaces/parameter samples: {num_surfaces:,}")
 
         # Draw parameters
-        lnvol = self.rng.uniform(0.05, 0.25, num_surfaces)
-        kappa = self.rng.uniform(0.25, 4.00, num_surfaces)
-        theta = self.rng.uniform(0.05**2, 0.25**2, num_surfaces)
-        xi = self.rng.uniform(0.10, 0.50, num_surfaces)
-        rho = self.rng.uniform(-0.40, 0.40, num_surfaces)
+        lnvol = self.rng.uniform(rg['LnVol'][0], rg['LnVol'][1], num_surfaces)
+        kappa = self.rng.uniform(rg['Kappa'][0], rg['Kappa'][1], num_surfaces)
+        theta = self.rng.uniform(rg['Theta'][0], rg['Theta'][1], num_surfaces)
+        xi = self.rng.uniform(rg['Xi'][0], rg['Xi'][1], num_surfaces)
+        rho = self.rng.uniform(rg['Rho'][0], rg['Rho'][1], num_surfaces)
 
         # Calculate prices per surface
         ts = []
         strikes = []
         fwds = []
         lnvols = []
         kappas = []
         thetas = []
         xis = []
         rhos = []
         prices = []
         for j in range(num_surfaces):
             print(f"Surface generation number {j+1:,}/{num_surfaces:,}")
-            expiries = self.rng.uniform(1.0 / 12.0, 5.0, self.num_expiries)
+            expiries = self.rng.uniform(rg['Ttm'][0], rg['Ttm'][1], self.num_expiries)
             # Need to sort these expiries
             expiries = np.unique(expiries)
-            fwd = self.rng.uniform(self.min_fwd, self.max_fwd, 1)[0]
+            fwd = self.rng.uniform(rg['F'][0], rg['F'][1], 1)[0]
             vol = lnvol[j]
 
             # Draw strikes
             ks = []
             for exp_idx in range(self.num_expiries):
                 # Spread method
                 # spread = self.rng.uniform(-300, 300, self.num_strikes)
                 # k = fwd + spread / 10000.0
                 # k = np.maximum(k, -shift + constants.BPS10)
 
                 # Percentile method
                 stdev = vol * np.sqrt(expiries[exp_idx])
-                percentiles = self.rng.uniform(0.01, 0.99, self.num_strikes)
+                percentiles = self.rng.uniform(rg['K'][0], rg['K'][1], self.num_strikes)
                 k = (fwd + shift) * np.exp(-0.5 * stdev * stdev + stdev * sp.norm.ppf(percentiles))
                 k = k - shift
 
                 ks.append(k)
 
             ks = np.asarray(ks)
 
@@ -131,20 +126,14 @@
         x_set = np.column_stack((t, strike, fwd, lnvol, kappa, theta, xi, rho))
         num_samples = len(nvol)
         y_set = np.asarray(nvol)
         y_set = np.reshape(y_set, (num_samples, 1))
 
         return x_set, y_set, data_df
 
-    # def price_surface_ref(self, expiries, strikes, is_call, fwd, parameters):
-    #     are_calls = [is_call] * strikes.shape[1]
-    #     are_calls = [are_calls] * expiries.shape[0]
-    #     ref_prices = self.price(expiries, strikes, are_calls, fwd, parameters)
-    #     return ref_prices
-
     def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         # Retrieve parameters
         lnvol = parameters['LnVol']
         kappa = parameters['Kappa']
         theta = parameters['Theta']
         xi = parameters['Xi']
         rho = parameters['Rho']
@@ -173,39 +162,38 @@
             expiry = point[0]
             strike = point[1]
             md_prices.append(bachelier.price(expiry, strike, is_call, fwd, vol))
 
         md_prices = np.asarray(md_prices)
         return md_prices.reshape(num_expiries, num_strikes)
 
-# Special class for Shifted Heston with shift = 3%, for easier calling
-class McShiftedHestonGenerator(McHestonGenerator):
-    """ For calling convenience, derived from McHestonGenerator with shift at typical 3%. """
-    def __init__(self, num_expiries=15, num_strikes=10, num_mc=10000, points_per_year=10):
-        McHestonGenerator.__init__(self, 0.03, num_expiries, num_strikes, num_mc, points_per_year)
-
 
 if __name__ == "__main__":
     NUM_SAMPLES = 100 #100 * 1000
-    NUM_MC = 100 * 1000
+    MODEL_TYPE = 'McHeston'
+    SHIFT = 0.03
+    NUM_MC = 1 * 1000
     POINTS_PER_YEAR = 25
     SURFACE_SIZE = 50
     NUM_EXPIRIES = 10
     NUM_STRIKES = int(SURFACE_SIZE / NUM_EXPIRIES)
-    MODEL_TYPE = 'McShiftedHeston'
     project_folder = os.path.join(settings.WORKFOLDER, "stovol")
     data_folder = os.path.join(project_folder, "samples")
     filemanager.check_directory(data_folder)
-    file = os.path.join(data_folder, MODEL_TYPE + "_samples.tsv")
-    generator = McShiftedHestonGenerator(NUM_EXPIRIES, NUM_STRIKES, NUM_MC, POINTS_PER_YEAR)
+    file = os.path.join(data_folder, MODEL_TYPE + "_samples_tests.tsv")
+    generator = McHestonGenerator(SHIFT, NUM_EXPIRIES, NUM_STRIKES, NUM_MC, POINTS_PER_YEAR)
 
+    ranges = {'Ttm': [1.0 / 12.0, 5.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041],
+              'LnVol': [0.05, 0.25], 'Kappa': [0.25, 4.00], 'Theta': [0.05**2, 0.25**2],
+              'Xi': [0.10, 0.50], 'Rho': [-0.40, 0.40]}
+    
     print("Generating " + str(NUM_SAMPLES) + " samples")
     gen_timer = timer.Stopwatch("Sample Generation")
     gen_timer.trigger()
-    data_df_ = generator.generate_samples(NUM_SAMPLES)
+    data_df_ = generator.generate_samples(NUM_SAMPLES, ranges)
     gen_timer.stop()
     print(data_df_)
     print("Cleansing data")
     nvol_timer = timer.Stopwatch("Convertion to normal vols")
     nvol_timer.trigger()
     data_df_ = generator.to_nvol(data_df_)
     nvol_timer.stop()
@@ -214,7 +202,28 @@
     file_timer.trigger()
     generator.to_file(data_df_, file)
     file_timer.stop()
     print("Complete!")
     gen_timer.print()
     nvol_timer.print()
     file_timer.print()
+
+    # Test ref surface calculation
+    # NUM_STRIKES = 100
+    # PARAMS = { 'LnVol': 0.20, 'Beta': 0.5, 'Nu': 0.55, 'Rho': -0.25, 'Gamma': 0.7, 'Kappa': 1.0,
+    #             'Theta': 0.05, 'Xi': 0.50 }
+    # FWD = 0.028
+
+    # # Any number of expiries can be calculated, but for optimum display choose no more than 6
+    # EXPIRIES = np.asarray([0.125, 0.250, 0.5, 1.00, 2.0, 5.0]).reshape(-1, 1)
+    # # EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
+    # NUM_EXPIRIES = EXPIRIES.shape[0]
+    # METHOD = 'Percentiles'
+    # PERCENTS = np.linspace(0.01, 0.99, num=NUM_STRIKES)
+    # PERCENTS = np.asarray([PERCENTS] * NUM_EXPIRIES)
+
+    # strikes = generator.convert_strikes(EXPIRIES, PERCENTS, FWD, PARAMS, METHOD)
+    # ARE_CALLS = [[False] * NUM_STRIKES] * NUM_EXPIRIES # All puts
+
+    # print("> Calculating chart surface with reference model")
+    # ref_prices = generator.price(EXPIRIES, strikes, ARE_CALLS, FWD, PARAMS)
+
```

### Comparing `sdevpy-0.1.3/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.1.4/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,178 +1,166 @@
-""" Smile generator for ZABR model using Monte-Carlo to calculate option prices """
+""" Smile generator for classic and shifted Hagan SABR models """
 import os
 import numpy as np
 import pandas as pd
 import scipy.stats as sp
 from sdevpy import settings
-from sdevpy.analytics import mczabr
-# from analytics import black
+from sdevpy.analytics import sabr
+from sdevpy.analytics import black
 from sdevpy.analytics import bachelier
-from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator
 from sdevpy.volsurfacegen.smilegenerator import SmileGenerator
 from sdevpy.tools import filemanager
-from sdevpy.tools import timer
 
 
-class McZabrGenerator(SabrGenerator):
-    """ ZABR model with a generic shift value, using Monte-Carlo to calculate option prices. """
-    def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, num_mc=10000,
-                 points_per_year=10):
-        SabrGenerator.__init__(self, shift)
-        # self.num_strikes = num_strikes
-        # self.num_expiries = num_expiries
-        # self.surface_size = self.num_expiries * self.num_strikes
-        self.num_mc = num_mc
-        self.points_per_year = points_per_year
-        # self.are_calls = [[self.is_call] * self.num_strikes] * self.num_expiries
+class SabrGenerator(SmileGenerator):
+    """ Base class for the classical SABR model. The classical Hagan model (non-shifted) is the
+        default case with shift = 0. """
+    def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, seed=42):
+        SmileGenerator.__init__(self, shift, num_expiries, num_strikes, seed)
 
-    def generate_samples(self, num_samples):
+    def generate_samples(self, num_samples, rg):
         shift = self.shift
 
         print(f"Number of strikes: {self.num_strikes:,}")
         print(f"Number of expiries: {self.num_expiries:,}")
         print(f"Surface size: {self.surface_size:,}")
         print(f"Number of samples: {num_samples:,}")
 
         # Derive number of surfaces to generate
         num_surfaces = int(num_samples / self.surface_size)# + 1)
         print(f"Number of surfaces/parameter samples: {num_surfaces:,}")
 
         # Draw parameters
-        lnvol = self.rng.uniform(0.05, 0.25, num_surfaces)
-        beta = self.rng.uniform(0.49, 0.51, num_surfaces)
-        nu = self.rng.uniform(0.20, 0.80, num_surfaces)
-        rho = self.rng.uniform(-0.40, 0.40, num_surfaces)
-        gamma = self.rng.uniform(0.10, 1.4, num_surfaces)
+        lnvol = self.rng.uniform(rg['LnVol'][0], rg['LnVol'][1], num_surfaces)
+        beta = self.rng.uniform(rg['Beta'][0], rg['Beta'][1], num_surfaces)
+        nu = self.rng.uniform(rg['Nu'][0], rg['Nu'][1], num_surfaces)
+        rho = self.rng.uniform(rg['Rho'][0], rg['Rho'][1], num_surfaces)
 
         # Calculate prices per surface
         ts = []
         strikes = []
         fwds = []
         lnvols = []
         betas = []
         nus = []
         rhos = []
-        gammas = []
         prices = []
         for j in range(num_surfaces):
             print(f"Surface generation number {j+1:,}/{num_surfaces:,}")
-            expiries = self.rng.uniform(1.0 / 12.0, 5.0, self.num_expiries)
+            expiries = self.rng.uniform(rg['Ttm'][0], rg['Ttm'][1], self.num_expiries)
             # Need to sort these expiries
             expiries = np.unique(expiries)
-            fwd = self.rng.uniform(self.min_fwd, self.max_fwd, 1)[0]
+            fwd = self.rng.uniform(rg['F'][0], rg['F'][1], 1)[0]
             vol = lnvol[j]
 
             # Draw strikes
             ks = []
             for exp_idx in range(self.num_expiries):
                 # Spread method
                 # spread = self.rng.uniform(-300, 300, self.num_strikes)
                 # k = fwd + spread / 10000.0
                 # k = np.maximum(k, -shift + constants.BPS10)
 
                 # Percentile method
                 stdev = vol * np.sqrt(expiries[exp_idx])
-                percentiles = self.rng.uniform(0.01, 0.99, self.num_strikes)
+                percentiles = self.rng.uniform(rg['K'][0], rg['K'][1], self.num_strikes)
                 k = (fwd + shift) * np.exp(-0.5 * stdev * stdev + stdev * sp.norm.ppf(percentiles))
                 k = k - shift
 
                 ks.append(k)
 
             ks = np.asarray(ks)
 
             # Draw parameters
-            params = {'LnVol': lnvol[j], 'Beta': beta[j], 'Nu': nu[j], 'Rho': rho[j],
-                      'Gamma': gamma[j]}
+            params = {'LnVol': lnvol[j], 'Beta': beta[j], 'Nu': nu[j], 'Rho': rho[j]}
 
             # Calculate prices
             price = self.price(expiries, ks, self.are_calls, fwd, params)
 
             # Flatten the results
             for exp_idx, expiry in enumerate(expiries):
                 ts.extend([expiry] * self.num_strikes)
                 strikes.extend(ks[exp_idx])
                 fwds.extend([fwd] * self.num_strikes)
                 lnvols.extend([lnvol[j]] * self.num_strikes)
                 betas.extend([beta[j]] * self.num_strikes)
                 nus.extend([nu[j]] * self.num_strikes)
                 rhos.extend([rho[j]] * self.num_strikes)
-                gammas.extend([gamma[j]] * self.num_strikes)
                 prices.extend(price[exp_idx])
 
         # Put in dataframe
         df = pd.DataFrame({'Ttm': ts, 'K': strikes, 'F': fwds, 'LnVol': lnvols, 'Beta': betas,
-                           'Nu': nus, 'Rho': rhos, 'Gamma': gammas, 'Price': prices})
-        df.columns = ['Ttm', 'K', 'F', 'LnVol', 'Beta', 'Nu', 'Rho', 'Gamma', 'Price']
+                           'Nu': nus, 'Rho': rhos, 'Price': prices})
+        df.columns = ['Ttm', 'K', 'F', 'LnVol', 'Beta', 'Nu', 'Rho', 'Price']
 
         return df
 
     def price(self, expiries, strikes, are_calls, fwd, parameters):
+        expiries_ = np.asarray(expiries).reshape(-1, 1)
         shifted_k = strikes + self.shift
         shifted_f = fwd + self.shift
-        prices = mczabr.price(expiries, shifted_k, are_calls, shifted_f, parameters,
-                              self.num_mc, self.points_per_year)
+        prices = []
+        for i, expiry in enumerate(expiries_):
+            k_prices = []
+            for j, sk in enumerate(shifted_k[i]):
+                iv = sabr.implied_vol_vec(expiry, sk, shifted_f, parameters)
+                price = black.price(expiry, sk, are_calls[i][j], shifted_f, iv)
+                k_prices.append(price[0])
+            prices.append(k_prices)
 
-        return prices
+        return np.asarray(prices)
 
     def retrieve_datasets(self, data_file, shuffle=False):
         data_df = SmileGenerator.from_file(data_file, shuffle)
 
         # Retrieve suitable data
         t = data_df.Ttm
         strike = data_df.K
         fwd = data_df.F
         lnvol = data_df.LnVol
         beta = data_df.Beta
         nu = data_df.Nu
         rho = data_df.Rho
-        gamma = data_df.Gamma
         nvol = data_df.NVol
 
         # Extract input and output datasets
-        x_set = np.column_stack((t, strike, fwd, lnvol, beta, nu, rho, gamma))
+        x_set = np.column_stack((t, strike, fwd, lnvol, beta, nu, rho))
         num_samples = len(nvol)
         y_set = np.asarray(nvol)
         y_set = np.reshape(y_set, (num_samples, 1))
 
         return x_set, y_set, data_df
 
-    # def price_surface_ref(self, expiries, strikes, is_call, fwd, parameters):
-    #     are_calls = [is_call] * strikes.shape[1]
-    #     are_calls = [are_calls] * expiries.shape[0]
-    #     ref_prices = self.price(expiries, strikes, are_calls, fwd, parameters)
-    #     return ref_prices
-
     def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         # Retrieve parameters
         lnvol = parameters['LnVol']
         beta = parameters['Beta']
         nu = parameters['Nu']
         rho = parameters['Rho']
-        gamma = parameters['Gamma']
 
         # Prepare learning model inputs
         num_expiries = expiries.shape[0]
         num_strikes = strikes.shape[1]
         num_points = num_expiries * num_strikes
-        md_inputs = np.ones((num_points, 8))
+        md_inputs = np.ones((num_points, 7))
         md_inputs[:, 0] = np.repeat(expiries, num_strikes)
         md_inputs[:, 1] = strikes.reshape(-1)
         md_inputs[:, 2] *= fwd
         md_inputs[:, 3] *= lnvol
         md_inputs[:, 4] *= beta
         md_inputs[:, 5] *= nu
         md_inputs[:, 6] *= rho
-        md_inputs[:, 7] *= gamma
 
         # Flatten are_calls
         flat_types = np.asarray(are_calls).reshape(-1)
 
-        # Price with learning model
+        # Get normal vol from learning model
         md_nvols = model.predict(md_inputs)
+
+        # Price with Bachelier
         md_prices = []
         for (point, vol, is_call) in zip(md_inputs, md_nvols, flat_types):
             expiry = point[0]
             strike = point[1]
             md_prices.append(bachelier.price(expiry, strike, is_call, fwd, vol))
 
         md_prices = np.asarray(md_prices)
@@ -184,48 +172,57 @@
     #         stdev = lnvol * np.sqrt(expiries)
     #         sfwd = fwd + self.shift
     #         return sfwd * np.exp(-0.5 * stdev**2 + stdev * sp.norm.ppf(strike_inputs)) - self.shift
     #     else:
     #         return SmileGenerator.convert_strikes(expiries, strike_inputs, fwd, parameters,
     #                                               input_method)
 
-# Special class for Shifted ZABR with shift = 3%, for easier calling
-class McShiftedZabrGenerator(McZabrGenerator):
-    """ For calling convenience, derived from McZabrGenerator with shift at typical 3%. """
-    def __init__(self, num_expiries=15, num_strikes=10, num_mc=10000, points_per_year=10):
-        McZabrGenerator.__init__(self, 0.03, num_expiries, num_strikes, num_mc, points_per_year)
-
 
 if __name__ == "__main__":
-    NUM_SAMPLES = 100 #100 * 1000
-    NUM_MC = 100 * 1000
-    POINTS_PER_YEAR = 25
-    SURFACE_SIZE = 50
-    NUM_EXPIRIES = 10
-    NUM_STRIKES = int(SURFACE_SIZE / NUM_EXPIRIES)
-    MODEL_TYPE = 'McShiftedZABR'
+    # Test generation
+    NUM_SAMPLES = 150 #100 * 1000
+    MODEL_TYPE = 'SABR'
+    SHIFT = 0.03
     project_folder = os.path.join(settings.WORKFOLDER, "stovol")
     data_folder = os.path.join(project_folder, "samples")
     filemanager.check_directory(data_folder)
-    file = os.path.join(data_folder, MODEL_TYPE + "_samples.tsv")
-    generator = McShiftedZabrGenerator(NUM_EXPIRIES, NUM_STRIKES, NUM_MC, POINTS_PER_YEAR)
+    file = os.path.join(data_folder, MODEL_TYPE + "_samples_test.tsv")
+    generator = SabrGenerator(SHIFT)
 
+    ranges = {'Ttm': [1.0 / 12.0, 35.0], 'K': [0.01, 0.99], 'F': [-0.009, 0.041],
+              'LnVol': [0.05, 0.50], 'Beta': [0.1, 0.9], 'Nu': [0.1, 1.0], 'Rho': [-0.6, 0.6]}
     print("Generating " + str(NUM_SAMPLES) + " samples")
-    gen_timer = timer.Stopwatch("Sample Generation")
-    gen_timer.trigger()
-    data_df_ = generator.generate_samples(NUM_SAMPLES)
-    gen_timer.stop()
+    data_df_ = generator.generate_samples(NUM_SAMPLES, ranges)
     print(data_df_)
     print("Cleansing data")
-    nvol_timer = timer.Stopwatch("Convertion to normal vols")
-    nvol_timer.trigger()
     data_df_ = generator.to_nvol(data_df_)
-    nvol_timer.stop()
     print("Output to file: " + file)
-    file_timer = timer.Stopwatch("Output to file")
-    file_timer.trigger()
     generator.to_file(data_df_, file)
-    file_timer.stop()
     print("Complete!")
-    gen_timer.print()
-    nvol_timer.print()
-    file_timer.print()
+
+    # Test price ref
+    # NUM_STRIKES = 100
+    # PARAMS = { 'LnVol': 0.20, 'Beta': 0.5, 'Nu': 0.55, 'Rho': -0.25 }
+    # FWD = 0.028
+
+    # # Any number of expiries can be calculated, but for optimum display choose no more than 6
+    # EXPIRIES = np.asarray([0.125, 0.250, 0.5, 1.00, 2.0, 5.0]).reshape(-1, 1)
+    # # EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
+    # NUM_EXPIRIES = EXPIRIES.shape[0]
+    # METHOD = 'Percentiles'
+    # PERCENTS = np.linspace(0.01, 0.99, num=NUM_STRIKES)
+    # PERCENTS = np.asarray([PERCENTS] * NUM_EXPIRIES)
+
+    # STRIKES = generator.convert_strikes(EXPIRIES, PERCENTS, FWD, PARAMS, METHOD)
+    # ARE_CALLS = [[False] * NUM_STRIKES] * NUM_EXPIRIES # All puts
+
+    # ref_prices = generator.price_surface_ref(EXPIRIES, STRIKES, ARE_CALLS, FWD, PARAMS)
+
+    # Test strike conversion
+    # generator = ShiftedSabrGenerator()
+    # EXPIRIES = np.asarray([0.5, 1.0, 5.0]).reshape(-1, 1)
+    # STRIKE_INPUTS = np.asarray([[0.1, 0.9], [0.4, 0.6], [0.5, 0.5]])
+    # FWD = 0.01
+    # PARAMETERS = { 'LnVol': 0.2222, 'Beta': 0.3333, 'Nu': 0.4444, 'Rho': -0.5555 }
+    # METHOD = 'Percentiles'
+    # prices = generator.price_surface_mod(None, EXPIRIES, STRIKE_INPUTS, FWD, PARAMETERS, METHOD)
+    # print(prices)
```

### Comparing `sdevpy-0.1.3/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.1.4/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,77 @@
 """ Base framework for smile generation """
 from abc import ABC, abstractmethod
 import numpy as np
 import pandas as pd
+import scipy.stats as sp
 from sdevpy.analytics import bachelier
 # from sdevpy.analytics import black
 
 
 class SmileGenerator(ABC):
     """ Base class for smile generation """
-    def __init__(self):
-        self.num_curve_parameters = 0
-        self.num_vol_parameters = 0
+    def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, seed=42):
+        # self.num_curve_parameters = 0
+        # self.num_vol_parameters = 0
         self.is_call = False  # Use put options by default
+        self.shift = shift
+        self.num_strikes = num_strikes
+        self.num_expiries = num_expiries
+        self.surface_size = self.num_expiries * self.num_strikes
+        self.are_calls = [[self.is_call] * self.num_strikes] * self.num_expiries
+        self.rng = np.random.RandomState(seed)
 
     @abstractmethod
-    def generate_samples(self, num_samples):
+    def generate_samples(self, num_samples, rg):
         """ Generate a sample of expiries, strikes, relevant parameters and option prices """
 
     @abstractmethod
     def price(self, expiries, strikes, are_calls, fwd, parameters):
         """ Calculate option price under the specified model and its parameters """
 
     @abstractmethod
     def retrieve_datasets(self, data_file, shuffle=False):
         """ Retrieve dataset stored in tsv file """
 
     # @abstractmethod
-    # def price_strike_ladder(self, model, expiry, spreads, fwd, parameters):
-    #     """ Calculate prices for a ladder of strikes for given parameters """
+    # def price_surface_ref(self, expiries, strikes, are_calls, fwd, parameters):
+    #     """ Calculate a surface of prices for given parameters using the generating model """
 
-    @abstractmethod
     def price_surface_ref(self, expiries, strikes, are_calls, fwd, parameters):
         """ Calculate a surface of prices for given parameters using the generating model """
+        return self.price(expiries, strikes, are_calls, fwd, parameters)
 
     @abstractmethod
     def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         """ Calculate a surface of prices for given parameters using the learning model """
 
     def convert_strikes(self, expiries, strike_inputs, fwd, parameters, input_method='Strikes'):
         """ Convert strike inputs into absolute strikes using the strike input_method """
+        # pylint: disable=unused-argument
         if input_method == 'Strikes':
             strikes = strike_inputs
         elif input_method == 'Spreads':
             strikes = fwd + strike_inputs / 10000.0
+        elif input_method == 'Percentiles':
+            if 'LnVol' in parameters:
+                lnvol = parameters['LnVol']
+                stdev = lnvol * np.sqrt(expiries)
+                sfwd = fwd + self.shift
+                N = sp.norm
+                return sfwd * np.exp(-0.5 * stdev**2 + stdev * N.ppf(strike_inputs)) - self.shift
+            else:
+                raise RuntimeError("Lognormal vol parameter not provided")
         else:
             raise ValueError("Invalid strike input method: " + input_method)
 
         return strikes
 
-    def num_parameters(self):
-        """ Total number of parameters (curve + vol) """
-        return self.num_curve_parameters + self.num_vol_parameters
+    # def num_parameters(self):
+    #     """ Total number of parameters (curve + vol) """
+    #     return self.num_curve_parameters + self.num_vol_parameters
 
     def to_nvol(self, data_df, cleanse=True, min_vol=0.0001, max_vol=0.1):
         """ Calculate normal implied vol and remove errors. Further remove points that are not
             in the given min/max range """
         # Calculate normal vols
         np.seterr(divide='raise')  # To catch errors and warnings
         t = data_df.Ttm
@@ -76,17 +93,19 @@
                 nvol.append(-9999)
 
         # Add test on Shifted BS
         # shift = 0.03
         # bsvol = []
         # for i in range(num_samples):
         #     if i % num_print == 0:
-        #         print(f"Converting to lognormal vol, batch {int(i/num_print)+1:,} out of {num_batches:,}")
+        #         print(f"Converting to lognormal vol, batch {int(i/num_print)+1:,} out of
+        #                   {num_batches:,}")
         #     try:
-        #         bsvol.append(black.implied_vol(t[i], strike[i] + shift, self.is_call, fwd[i] + shift, price[i]))
+        #         bsvol.append(black.implied_vol(t[i], strike[i] + shift, self.is_call,
+        #                    fwd[i] + shift, price[i]))
         #     except (Exception,):
         #         bsvol.append(-9999)
 
 
         np.seterr(divide='warn')  # Set back to warning
 
         data_df['NVol'] = nvol
```

### Comparing `sdevpy-0.1.3/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.1.4/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 """ Select stovol generator based on type and other required information """
-from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator, ShiftedSabrGenerator
-from sdevpy.volsurfacegen.mcsabrgenerator import McShiftedSabrGenerator
+from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator
+from sdevpy.volsurfacegen.mcsabrgenerator import McSabrGenerator
 from sdevpy.volsurfacegen.fbsabrgenerator import FbSabrGenerator
-from sdevpy.volsurfacegen.mczabrgenerator import McShiftedZabrGenerator
-from sdevpy.volsurfacegen.mchestongenerator import McShiftedHestonGenerator
+from sdevpy.volsurfacegen.mczabrgenerator import McZabrGenerator
+from sdevpy.volsurfacegen.mchestongenerator import McHestonGenerator
 
 
-def set_generator(type_, num_expiries=10, surface_size=50, num_mc=100000,
+def set_generator(type_, shift=0.03, num_expiries=10, num_strikes=5, num_mc=100000,
                   points_per_year=25, seed=42):
     """ Select generator based on type and other information. Currently available are: SABR,
-        ShiftedSABR, McShiftedSABR, FbSABR, McShiftedZABR and McShiftedHeston. All models
-        except SABR and ShiftedSABR require inputs num_expiries and surface_size for sample
-        generation, and num_mc and points_per_year for price calculation.
-    """
-    num_strikes = int(surface_size / num_expiries)
-
+        McSABR, FbSABR, McZABR and McHeston. """
     if type_ == "SABR":
-        generator = SabrGenerator(0.0, num_expiries, num_strikes, seed)
-    elif type_ == "ShiftedSABR":
-        generator = ShiftedSabrGenerator(num_expiries, num_strikes, seed)
-    elif type_ == "McShiftedSABR":
-        generator = McShiftedSabrGenerator(num_expiries, num_strikes, num_mc, points_per_year)
+        generator = SabrGenerator(shift, num_expiries, num_strikes, seed)
+    elif type_ == "McSABR":
+        generator = McSabrGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year)
     elif type_ == "FbSABR":
         generator = FbSabrGenerator(num_expiries, num_strikes, num_mc, points_per_year)
-    elif type_ == "McShiftedZABR":
-        generator = McShiftedZabrGenerator(num_expiries, num_strikes, num_mc, points_per_year)
-    elif type_ == "McShiftedHeston":
-        generator = McShiftedHestonGenerator(num_expiries, num_strikes, num_mc, points_per_year)
+    elif type_ == "McZABR":
+        generator = McZabrGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year)
+    elif type_ == "McHeston":
+        generator = McHestonGenerator(shift, num_expiries, num_strikes, num_mc, points_per_year)
     else:
         raise ValueError("Unknown model: " + type_)
 
     return generator
 
 if __name__ == "__main__":
-    NUM_MC = 100 * 1000
+    NUM_MC = 1 * 1000
     POINTS_PER_YEAR = 25
-    SURFACE_SIZE = 50
     NUM_EXPIRIES = 10
+    NUM_STRIKES = 5
     TYPE = 'FbSABR'
-    GENERATOR = set_generator(TYPE, NUM_EXPIRIES, SURFACE_SIZE, NUM_MC, POINTS_PER_YEAR)
+    SHIFT = 0.03
+    GENERATOR = set_generator(TYPE, SHIFT, NUM_EXPIRIES, NUM_STRIKES, NUM_MC, POINTS_PER_YEAR)
 
     print("Setting generator model " + TYPE)
     print("Complete!")
```

### Comparing `sdevpy-0.1.3/src/sdevpy.egg-info/PKG-INFO` & `sdevpy-0.1.4/src/sdevpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.1.3/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.1.4/src/sdevpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 src/sdevpy/projects/datafiles.py
 src/sdevpy/projects/pinns/ernst_pinns.py
 src/sdevpy/projects/pinns/pinns.py
 src/sdevpy/projects/pinns/pinns_worst_of.py
 src/sdevpy/projects/stovol/stovolgen.py
 src/sdevpy/projects/stovol/stovolplot.py
 src/sdevpy/projects/stovol/stovoltrain.py
-src/sdevpy/projects/stovol/xsabrfit.py
 src/sdevpy/tools/clipboard.py
 src/sdevpy/tools/constants.py
 src/sdevpy/tools/filemanager.py
 src/sdevpy/tools/jsonmanager.py
 src/sdevpy/tools/timegrids.py
 src/sdevpy/tools/timer.py
 src/sdevpy/volsurfacegen/fbsabrgenerator.py
```

