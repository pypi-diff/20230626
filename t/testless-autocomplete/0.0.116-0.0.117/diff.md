# Comparing `tmp/testless_autocomplete-0.0.116.tar.gz` & `tmp/testless_autocomplete-0.0.117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_autocomplete-0.0.116.tar", last modified: Mon Jun 26 16:41:32 2023, max compression
+gzip compressed data, was "testless_autocomplete-0.0.117.tar", last modified: Mon Jun 26 16:44:15 2023, max compression
```

## Comparing `testless_autocomplete-0.0.116.tar` & `testless_autocomplete-0.0.117.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:41:32.345585 testless_autocomplete-0.0.116/
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:41:32.341653 testless_autocomplete-0.0.116/Auto_Complete/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-22 21:16:29.000000 testless_autocomplete-0.0.116/Auto_Complete/__init__.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:41:32.343328 testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      560 2023-06-25 21:09:29.000000 testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      184 2023-06-25 20:08:40.000000 testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/__init__.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-22 21:50:10.000000 testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/model.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-22 21:40:11.000000 testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/ngram.csv
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-22 21:39:36.000000 testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/preprocessing.py
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       54 2023-06-25 20:27:59.000000 testless_autocomplete-0.0.116/MANIFEST.in
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-26 16:41:32.345410 testless_autocomplete-0.0.116/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-22 21:27:54.000000 testless_autocomplete-0.0.116/README.md
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-26 16:41:32.345628 testless_autocomplete-0.0.116/setup.cfg
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      795 2023-06-26 16:41:04.000000 testless_autocomplete-0.0.116/setup.py
-drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:41:32.345232 testless_autocomplete-0.0.116/testless_autocomplete.egg-info/
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      337 2023-06-26 16:41:32.000000 testless_autocomplete-0.0.116/testless_autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      527 2023-06-26 16:41:32.000000 testless_autocomplete-0.0.116/testless_autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        1 2023-06-26 16:41:32.000000 testless_autocomplete-0.0.116/testless_autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       45 2023-06-26 16:41:32.000000 testless_autocomplete-0.0.116/testless_autocomplete.egg-info/requires.txt
--rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       14 2023-06-26 16:41:32.000000 testless_autocomplete-0.0.116/testless_autocomplete.egg-info/top_level.txt
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:44:15.217336 testless_autocomplete-0.0.117/
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:44:15.214599 testless_autocomplete-0.0.117/Auto_Complete/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-22 21:16:29.000000 testless_autocomplete-0.0.117/Auto_Complete/__init__.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:44:15.215898 testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      560 2023-06-25 21:09:29.000000 testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      184 2023-06-25 20:08:40.000000 testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/__init__.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)     1262 2023-06-22 21:50:10.000000 testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/model.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)    12483 2023-06-22 21:40:11.000000 testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/ngram.csv
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      756 2023-06-22 21:39:36.000000 testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/preprocessing.py
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       54 2023-06-25 20:27:59.000000 testless_autocomplete-0.0.117/MANIFEST.in
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      369 2023-06-26 16:44:15.217119 testless_autocomplete-0.0.117/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       38 2023-06-26 16:44:15.217388 testless_autocomplete-0.0.117/setup.cfg
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      746 2023-06-26 16:44:10.000000 testless_autocomplete-0.0.117/setup.py
+drwxr-xr-x   0 eng-mostafamagdy   (501) staff       (20)        0 2023-06-26 16:44:15.216856 testless_autocomplete-0.0.117/testless_autocomplete.egg-info/
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      369 2023-06-26 16:44:15.000000 testless_autocomplete-0.0.117/testless_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)      517 2023-06-26 16:44:15.000000 testless_autocomplete-0.0.117/testless_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)        1 2023-06-26 16:44:15.000000 testless_autocomplete-0.0.117/testless_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       45 2023-06-26 16:44:15.000000 testless_autocomplete-0.0.117/testless_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 eng-mostafamagdy   (501) staff       (20)       14 2023-06-26 16:44:15.000000 testless_autocomplete-0.0.117/testless_autocomplete.egg-info/top_level.txt
```

### Comparing `testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py` & `testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/AutoCompleteAPI.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/model.py` & `testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/model.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/ngram.csv` & `testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/ngram.csv`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.116/Auto_Complete/testless_autocomplete/preprocessing.py` & `testless_autocomplete-0.0.117/Auto_Complete/testless_autocomplete/preprocessing.py`

 * *Files identical despite different names*

### Comparing `testless_autocomplete-0.0.116/setup.py` & `testless_autocomplete-0.0.117/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import find_packages, setup
 
-with open("README.md", "r") as f:
-    long_description = f.read()
+
 
 setup(
     name="testless_autocomplete",
-    version="0.0.116",
+    version="0.0.117",
     description="Auto Complete Package",
     packages=find_packages(),
-    long_description=long_description,
+    long_description="TestLess Auto Complete Package",
     long_description_content_type="text/markdown",
     author="TestLess",
     package_data={
         '/Auto_Complete': ['/testless_autocomplete/ngram.csv'],
     },
     include_package_data=True,
     license="MIT",
```

### Comparing `testless_autocomplete-0.0.116/testless_autocomplete.egg-info/SOURCES.txt` & `testless_autocomplete-0.0.117/testless_autocomplete.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 MANIFEST.in
-README.md
 setup.py
 Auto_Complete/__init__.py
 Auto_Complete/testless_autocomplete/AutoCompleteAPI.py
 Auto_Complete/testless_autocomplete/__init__.py
 Auto_Complete/testless_autocomplete/model.py
 Auto_Complete/testless_autocomplete/ngram.csv
 Auto_Complete/testless_autocomplete/preprocessing.py
```

