# Comparing `tmp/ChemCal-0.0.2.tar.gz` & `tmp/ChemCal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChemCal-0.0.2.tar", last modified: Fri Jun 23 09:23:34 2023, max compression
+gzip compressed data, was "ChemCal-0.0.4.tar", last modified: Mon Jun 26 05:10:44 2023, max compression
```

## Comparing `ChemCal-0.0.2.tar` & `ChemCal-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-23 09:23:34.314898 ChemCal-0.0.2/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-23 09:23:34.314898 ChemCal-0.0.2/ChemCal/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-23 09:23:31.000000 ChemCal-0.0.2/ChemCal/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2841 2023-06-23 09:23:31.000000 ChemCal-0.0.2/ChemCal/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3210 2023-06-23 09:23:31.000000 ChemCal-0.0.2/ChemCal/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-23 09:23:34.314898 ChemCal-0.0.2/ChemCal.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     6809 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      324 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       36 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-21 23:54:27.000000 ChemCal-0.0.2/ChemCal.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        8 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-21 23:43:34.000000 ChemCal-0.0.2/LICENSE
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 ChemCal-0.0.2/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     6809 2023-06-23 09:23:34.314898 ChemCal-0.0.2/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     5977 2023-06-23 09:14:10.000000 ChemCal-0.0.2/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      933 2023-06-23 09:23:31.000000 ChemCal-0.0.2/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-23 09:23:34.314898 ChemCal-0.0.2/setup.cfg
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 ChemCal-0.0.2/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-26 05:10:44.730143 ChemCal-0.0.4/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-26 05:10:44.730143 ChemCal-0.0.4/ChemCal/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-26 05:10:34.000000 ChemCal-0.0.4/ChemCal/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3111 2023-06-26 05:10:34.000000 ChemCal-0.0.4/ChemCal/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     6629 2023-06-26 05:10:34.000000 ChemCal-0.0.4/ChemCal/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-26 05:10:44.730143 ChemCal-0.0.4/ChemCal.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2567 2023-06-26 05:10:44.000000 ChemCal-0.0.4/ChemCal.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      324 2023-06-26 05:10:44.000000 ChemCal-0.0.4/ChemCal.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-26 05:10:44.000000 ChemCal-0.0.4/ChemCal.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       36 2023-06-26 05:10:44.000000 ChemCal-0.0.4/ChemCal.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-21 23:54:27.000000 ChemCal-0.0.4/ChemCal.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-26 05:10:44.000000 ChemCal-0.0.4/ChemCal.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        8 2023-06-26 05:10:44.000000 ChemCal-0.0.4/ChemCal.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-21 23:43:34.000000 ChemCal-0.0.4/LICENSE
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 ChemCal-0.0.4/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2567 2023-06-26 05:10:44.730143 ChemCal-0.0.4/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1735 2023-06-26 05:10:37.000000 ChemCal-0.0.4/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      933 2023-06-26 05:10:27.000000 ChemCal-0.0.4/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-26 05:10:44.730143 ChemCal-0.0.4/setup.cfg
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 ChemCal-0.0.4/setup.py
```

### Comparing `ChemCal-0.0.2/ChemCal/_modidx.py` & `ChemCal-0.0.4/ChemCal/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
                                                                                'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_sxhat': ( 'core.html#calibrationmodel.calculate_sxhat',
                                                                                  'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_syx': ( 'core.html#calibrationmodel.calculate_syx',
                                                                                'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_uncertainty': ( 'core.html#calibrationmodel.calculate_uncertainty',
                                                                                        'ChemCal/core.py'),
+                              'ChemCal.core.CalibrationModel.calplot': ('core.html#calibrationmodel.calplot', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.fit_model': ('core.html#calibrationmodel.fit_model', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.fit_ols': ('core.html#calibrationmodel.fit_ols', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.get_t_value': ('core.html#calibrationmodel.get_t_value', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.inverse_prediction': ( 'core.html#calibrationmodel.inverse_prediction',
                                                                                     'ChemCal/core.py'),
+                              'ChemCal.core.CalibrationModel.linest_stats': ('core.html#calibrationmodel.linest_stats', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.tabulate_results': ( 'core.html#calibrationmodel.tabulate_results',
                                                                                   'ChemCal/core.py')}}}
```

### Comparing `ChemCal-0.0.2/LICENSE` & `ChemCal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ChemCal-0.0.2/settings.ini` & `ChemCal-0.0.4/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ChemCal
 lib_name = ChemCal
-version = 0.0.2
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ChemCal
 nbs_path = nbs
 recursive = True
```

### Comparing `ChemCal-0.0.2/setup.py` & `ChemCal-0.0.4/setup.py`

 * *Files identical despite different names*

