# Comparing `tmp/madml-0.0.5.tar.gz` & `tmp/madml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madml-0.0.5.tar", last modified: Mon Jun 26 16:15:57 2023, max compression
+gzip compressed data, was "madml-0.0.6.tar", last modified: Mon Jun 26 16:25:30 2023, max compression
```

## Comparing `madml-0.0.5.tar` & `madml-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.907232 madml-0.0.5/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1097 2023-06-26 14:22:33.000000 madml-0.0.5/LICENSE
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3690 2023-06-26 16:15:57.907232 madml-0.0.5/PKG-INFO
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3182 2023-06-26 15:58:15.000000 madml-0.0.5/README.md
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      142 2023-06-26 15:56:15.000000 madml-0.0.5/pyproject.toml
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       38 2023-06-26 16:15:57.907232 madml-0.0.5/setup.cfg
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1584 2023-06-26 16:15:49.000000 madml-0.0.5/setup.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.903231 madml-0.0.5/src/
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.903231 madml-0.0.5/src/madml/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/__init__.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     5812 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/datasets.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.903231 madml-0.0.5/src/madml/hosting/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:00.000000 madml-0.0.5/src/madml/hosting/__init__.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1274 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/hosting/docker.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.903231 madml-0.0.5/src/madml/ml/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/ml/__init__.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     4752 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/ml/assessment.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     4070 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/ml/splitters.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.907232 madml-0.0.5/src/madml/models/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/models/__init__.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     9312 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/models/combine.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     2107 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/models/space.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3121 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/models/uq.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)    33226 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/plots.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      840 2023-06-26 14:22:33.000000 madml-0.0.5/src/madml/utils.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.903231 madml-0.0.5/src/madml.egg-info/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3690 2023-06-26 16:15:57.000000 madml-0.0.5/src/madml.egg-info/PKG-INFO
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      571 2023-06-26 16:15:57.000000 madml-0.0.5/src/madml.egg-info/SOURCES.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 16:15:57.000000 madml-0.0.5/src/madml.egg-info/dependency_links.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       78 2023-06-26 16:15:57.000000 madml-0.0.5/src/madml.egg-info/requires.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        6 2023-06-26 16:15:57.000000 madml-0.0.5/src/madml.egg-info/top_level.txt
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:57.907232 madml-0.0.5/tests/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      318 2023-06-26 14:22:33.000000 madml-0.0.5/tests/test_load_data.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1899 2023-06-26 14:22:33.000000 madml-0.0.5/tests/test_run.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1097 2023-06-26 14:22:33.000000 madml-0.0.6/LICENSE
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3690 2023-06-26 16:25:30.169482 madml-0.0.6/PKG-INFO
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3182 2023-06-26 15:58:15.000000 madml-0.0.6/README.md
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      142 2023-06-26 15:56:15.000000 madml-0.0.6/pyproject.toml
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)       38 2023-06-26 16:25:30.169482 madml-0.0.6/setup.cfg
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1584 2023-06-26 16:19:30.000000 madml-0.0.6/setup.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.165482 madml-0.0.6/src/
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/src/madml/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/__init__.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/src/madml/data/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:14.000000 madml-0.0.6/src/madml/data/__init__.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     5812 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/datasets.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/src/madml/hosting/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:15:00.000000 madml-0.0.6/src/madml/hosting/__init__.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1274 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/hosting/docker.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/src/madml/ml/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/ml/__init__.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     4752 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/ml/assessment.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     4070 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/ml/splitters.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/src/madml/models/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        0 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/models/__init__.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     9312 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/models/combine.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     2107 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/models/space.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3121 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/models/uq.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)    33226 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/plots.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      840 2023-06-26 14:22:33.000000 madml-0.0.6/src/madml/utils.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/src/madml.egg-info/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3690 2023-06-26 16:25:30.000000 madml-0.0.6/src/madml.egg-info/PKG-INFO
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      598 2023-06-26 16:25:30.000000 madml-0.0.6/src/madml.egg-info/SOURCES.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 16:25:30.000000 madml-0.0.6/src/madml.egg-info/dependency_links.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)       78 2023-06-26 16:25:30.000000 madml-0.0.6/src/madml.egg-info/requires.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        6 2023-06-26 16:25:30.000000 madml-0.0.6/src/madml.egg-info/top_level.txt
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 16:25:30.169482 madml-0.0.6/tests/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      318 2023-06-26 14:22:33.000000 madml-0.0.6/tests/test_load_data.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1899 2023-06-26 14:22:33.000000 madml-0.0.6/tests/test_run.py
```

### Comparing `madml-0.0.5/LICENSE` & `madml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/PKG-INFO` & `madml-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madml
-Version: 0.0.5
+Version: 0.0.6
 Summary: Application domain of machine learning in materials science.
 Home-page: https://github.com/leschultz/materials_application_domain_machine_learning.git
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_qwqq5vnx_/tmpf4000g1j_TarContainer/0/2", line 99, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_qwqq5vnx_/tmpf4000g1j_TarContainer/0/2", line 99, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: madml Version: 0.0.5 Summary: Application domain of
+Metadata-Version: 2.1 Name: madml Version: 0.0.6 Summary: Application domain of
 machine learning in materials science. Home-page: https://github.com/leschultz/
 materials_application_domain_machine_learning.git Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE # Materials Application Domain
 Machine Learning (MADML) Research with respect to application domain with a
```

### Comparing `madml-0.0.5/README.md` & `madml-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/setup.py` & `madml-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 # Package information
 name = 'madml'
-version = '0.0.5'
+version = '0.0.6'
 description = 'Application domain of machine learning in materials science.'
 url = 'https://github.com/leschultz/'\
       'materials_application_domain_machine_learning.git'
 author = 'Lane E. Schultz'
 author_email = 'laneenriqueschultz@gmail.com'
 python_requires = '>=3.6'
 classifiers = ['Programming Language :: Python :: 3',
```

### Comparing `madml-0.0.5/src/madml/datasets.py` & `madml-0.0.6/src/madml/datasets.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/hosting/docker.py` & `madml-0.0.6/src/madml/hosting/docker.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/ml/assessment.py` & `madml-0.0.6/src/madml/ml/assessment.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/ml/splitters.py` & `madml-0.0.6/src/madml/ml/splitters.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/models/combine.py` & `madml-0.0.6/src/madml/models/combine.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/models/space.py` & `madml-0.0.6/src/madml/models/space.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/models/uq.py` & `madml-0.0.6/src/madml/models/uq.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/plots.py` & `madml-0.0.6/src/madml/plots.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml/utils.py` & `madml-0.0.6/src/madml/utils.py`

 * *Files identical despite different names*

### Comparing `madml-0.0.5/src/madml.egg-info/PKG-INFO` & `madml-0.0.6/src/madml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madml
-Version: 0.0.5
+Version: 0.0.6
 Summary: Application domain of machine learning in materials science.
 Home-page: https://github.com/leschultz/materials_application_domain_machine_learning.git
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_qwqq5vnx_/tmpf4000g1j_TarContainer/0/26", line 99, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_qwqq5vnx_/tmpf4000g1j_TarContainer/0/26", line 99, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: madml Version: 0.0.5 Summary: Application domain of
+Metadata-Version: 2.1 Name: madml Version: 0.0.6 Summary: Application domain of
 machine learning in materials science. Home-page: https://github.com/leschultz/
 materials_application_domain_machine_learning.git Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE # Materials Application Domain
 Machine Learning (MADML) Research with respect to application domain with a
```

### Comparing `madml-0.0.5/src/madml.egg-info/SOURCES.txt` & `madml-0.0.6/src/madml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/madml/plots.py
 src/madml/utils.py
 src/madml.egg-info/PKG-INFO
 src/madml.egg-info/SOURCES.txt
 src/madml.egg-info/dependency_links.txt
 src/madml.egg-info/requires.txt
 src/madml.egg-info/top_level.txt
+src/madml/data/__init__.py
 src/madml/hosting/__init__.py
 src/madml/hosting/docker.py
 src/madml/ml/__init__.py
 src/madml/ml/assessment.py
 src/madml/ml/splitters.py
 src/madml/models/__init__.py
 src/madml/models/combine.py
```

### Comparing `madml-0.0.5/tests/test_run.py` & `madml-0.0.6/tests/test_run.py`

 * *Files identical despite different names*

