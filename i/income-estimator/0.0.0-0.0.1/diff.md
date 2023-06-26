# Comparing `tmp/income_estimator-0.0.0.tar.gz` & `tmp/income_estimator-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "income_estimator-0.0.0.tar", last modified: Mon Jun 26 19:30:14 2023, max compression
+gzip compressed data, was "income_estimator-0.0.1.tar", last modified: Mon Jun 26 20:16:24 2023, max compression
```

## Comparing `income_estimator-0.0.0.tar` & `income_estimator-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 19:30:14.373179 income_estimator-0.0.0/
--rw-rw-rw-   0        0        0     2976 2023-06-26 19:20:43.000000 income_estimator-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       59 2023-06-26 19:00:05.000000 income_estimator-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4050 2023-06-26 19:30:14.373179 income_estimator-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-06-26 19:21:30.000000 income_estimator-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 19:30:14.355179 income_estimator-0.0.0/income_estimator/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:51:35.000000 income_estimator-0.0.0/income_estimator/__init__.py
--rw-rw-rw-   0        0        0     6487 2023-06-26 18:44:51.000000 income_estimator-0.0.0/income_estimator/income_estimator.py
--rw-rw-rw-   0        0        0     1210 2023-06-26 17:44:38.000000 income_estimator-0.0.0/income_estimator/usd_string_class.py
-drwxrwxrwx   0        0        0        0 2023-06-26 19:30:14.371179 income_estimator-0.0.0/income_estimator.egg-info/
--rw-rw-rw-   0        0        0     4050 2023-06-26 19:30:14.000000 income_estimator-0.0.0/income_estimator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-26 19:30:14.000000 income_estimator-0.0.0/income_estimator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 19:30:14.000000 income_estimator-0.0.0/income_estimator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-26 19:30:14.000000 income_estimator-0.0.0/income_estimator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      905 2023-06-26 19:30:00.000000 income_estimator-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 19:30:14.374179 income_estimator-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-06-26 18:52:28.000000 income_estimator-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:16:24.810149 income_estimator-0.0.1/
+-rw-rw-rw-   0        0        0     2976 2023-06-26 19:20:43.000000 income_estimator-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-06-26 19:00:05.000000 income_estimator-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4406 2023-06-26 20:16:24.809124 income_estimator-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-06-26 19:21:30.000000 income_estimator-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:16:24.788150 income_estimator-0.0.1/income_estimator/
+-rw-rw-rw-   0        0        0        0 2023-06-26 18:51:35.000000 income_estimator-0.0.1/income_estimator/__init__.py
+-rw-rw-rw-   0        0        0     6487 2023-06-26 18:44:51.000000 income_estimator-0.0.1/income_estimator/income_estimator.py
+-rw-rw-rw-   0        0        0     1210 2023-06-26 17:44:38.000000 income_estimator-0.0.1/income_estimator/usd_string_class.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:16:24.808125 income_estimator-0.0.1/income_estimator.egg-info/
+-rw-rw-rw-   0        0        0     4406 2023-06-26 20:16:24.000000 income_estimator-0.0.1/income_estimator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-26 20:16:24.000000 income_estimator-0.0.1/income_estimator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:16:24.000000 income_estimator-0.0.1/income_estimator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 20:16:24.000000 income_estimator-0.0.1/income_estimator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1239 2023-06-26 20:16:09.000000 income_estimator-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:16:24.810149 income_estimator-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-06-26 18:52:28.000000 income_estimator-0.0.1/setup.py
```

### Comparing `income_estimator-0.0.0/LICENSE` & `income_estimator-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `income_estimator-0.0.0/PKG-INFO` & `income_estimator-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: income_estimator
-Version: 0.0.0
+Version: 0.0.1
 Summary: Proprietary Python 3.7 package to be used by for Bronsoneering purposes, by permitted personnel.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: BRONSONEERING LLC END USER LICENSE AGREEMENT (EULA)
         
         Preamble:
         By accepting this End User License Agreement (“EULA” or this “Agreement,” inclusive of the Addendums annexed hereto) or
         by downloading or using the software you signify that you have read and agree to all the terms of this Agreement, as it
@@ -39,14 +39,18 @@
         unauthorized access, copying or downloading. Accordingly, the parties agree that Bronsoneering will not be liable for
         any third-party use of the User Creative unless such use is both wrongful and expressly authorized in writing by
         Bronsoneering.
         
         Bronsoneering LLC
         bronsoneering@gmail.com
         
+Project-URL: Homepage, https://github.com/helloDestroyerOfWorlds/income_estimator.git
+Project-URL: Documentation, https://github.com/helloDestroyerOfWorlds/income_estimator.git
+Project-URL: Repository, https://github.com/helloDestroyerOfWorlds/income_estimator.git
+Project-URL: Changelog, https://github.com/helloDestroyerOfWorlds/income_estimator.git
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 1 - Planning
```

### Comparing `income_estimator-0.0.0/income_estimator/income_estimator.py` & `income_estimator-0.0.1/income_estimator/income_estimator.py`

 * *Files identical despite different names*

### Comparing `income_estimator-0.0.0/income_estimator/usd_string_class.py` & `income_estimator-0.0.1/income_estimator/usd_string_class.py`

 * *Files identical despite different names*

### Comparing `income_estimator-0.0.0/income_estimator.egg-info/PKG-INFO` & `income_estimator-0.0.1/income_estimator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: income-estimator
-Version: 0.0.0
+Version: 0.0.1
 Summary: Proprietary Python 3.7 package to be used by for Bronsoneering purposes, by permitted personnel.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: BRONSONEERING LLC END USER LICENSE AGREEMENT (EULA)
         
         Preamble:
         By accepting this End User License Agreement (“EULA” or this “Agreement,” inclusive of the Addendums annexed hereto) or
         by downloading or using the software you signify that you have read and agree to all the terms of this Agreement, as it
@@ -39,14 +39,18 @@
         unauthorized access, copying or downloading. Accordingly, the parties agree that Bronsoneering will not be liable for
         any third-party use of the User Creative unless such use is both wrongful and expressly authorized in writing by
         Bronsoneering.
         
         Bronsoneering LLC
         bronsoneering@gmail.com
         
+Project-URL: Homepage, https://github.com/helloDestroyerOfWorlds/income_estimator.git
+Project-URL: Documentation, https://github.com/helloDestroyerOfWorlds/income_estimator.git
+Project-URL: Repository, https://github.com/helloDestroyerOfWorlds/income_estimator.git
+Project-URL: Changelog, https://github.com/helloDestroyerOfWorlds/income_estimator.git
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 1 - Planning
```

