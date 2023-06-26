# Comparing `tmp/madml-0.0.1.tar.gz` & `tmp/madml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madml-0.0.1.tar", last modified: Mon Jun 26 15:15:16 2023, max compression
+gzip compressed data, was "madml-0.0.2.tar", last modified: Mon Jun 26 15:57:07 2023, max compression
```

## Comparing `madml-0.0.1.tar` & `madml-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:15:16.849252 madml-0.0.1/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1097 2023-06-26 14:22:33.000000 madml-0.0.1/LICENSE
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3671 2023-06-26 15:15:16.849252 madml-0.0.1/PKG-INFO
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3163 2023-06-26 15:04:33.000000 madml-0.0.1/README.md
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:15:16.849252 madml-0.0.1/madml.egg-info/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     3671 2023-06-26 15:15:16.000000 madml-0.0.1/madml.egg-info/PKG-INFO
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      227 2023-06-26 15:15:16.000000 madml-0.0.1/madml.egg-info/SOURCES.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 15:15:16.000000 madml-0.0.1/madml.egg-info/dependency_links.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       78 2023-06-26 15:15:16.000000 madml-0.0.1/madml.egg-info/requires.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 15:15:16.000000 madml-0.0.1/madml.egg-info/top_level.txt
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       94 2023-06-26 14:28:37.000000 madml-0.0.1/pyproject.toml
--rw-rw-r--   0 nerve     (1000) nerve     (1000)       38 2023-06-26 15:15:16.849252 madml-0.0.1/setup.cfg
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1531 2023-06-26 15:15:10.000000 madml-0.0.1/setup.py
-drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:15:16.849252 madml-0.0.1/tests/
--rw-rw-r--   0 nerve     (1000) nerve     (1000)      318 2023-06-26 14:22:33.000000 madml-0.0.1/tests/test_load_data.py
--rw-rw-r--   0 nerve     (1000) nerve     (1000)     1899 2023-06-26 14:22:33.000000 madml-0.0.1/tests/test_run.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:57:07.698796 madml-0.0.2/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1097 2023-06-26 14:22:33.000000 madml-0.0.2/LICENSE
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3671 2023-06-26 15:57:07.698796 madml-0.0.2/PKG-INFO
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3163 2023-06-26 15:04:33.000000 madml-0.0.2/README.md
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:57:07.694796 madml-0.0.2/madml.egg-info/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     3671 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/PKG-INFO
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      227 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/SOURCES.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/dependency_links.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)       78 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/requires.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)        1 2023-06-26 15:57:07.000000 madml-0.0.2/madml.egg-info/top_level.txt
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      142 2023-06-26 15:56:15.000000 madml-0.0.2/pyproject.toml
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)       38 2023-06-26 15:57:07.698796 madml-0.0.2/setup.cfg
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1531 2023-06-26 15:56:54.000000 madml-0.0.2/setup.py
+drwxrwxr-x   0 nerve     (1000) nerve     (1000)        0 2023-06-26 15:57:07.694796 madml-0.0.2/tests/
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)      318 2023-06-26 14:22:33.000000 madml-0.0.2/tests/test_load_data.py
+-rw-rw-r--   0 nerve     (1000) nerve     (1000)     1899 2023-06-26 14:22:33.000000 madml-0.0.2/tests/test_run.py
```

### Comparing `madml-0.0.1/LICENSE` & `madml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `madml-0.0.1/PKG-INFO` & `madml-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madml
-Version: 0.0.1
+Version: 0.0.2
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

 * *File "/tmp/diffoscope_h8o7bnlb_/tmp96vh1czb_TarContainer/0/2", line 99, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_h8o7bnlb_/tmp96vh1czb_TarContainer/0/2", line 99, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: madml Version: 0.0.1 Summary: Application domain of
+Metadata-Version: 2.1 Name: madml Version: 0.0.2 Summary: Application domain of
 machine learning in materials science. Home-page: https://github.com/leschultz/
 materials_application_domain_machine_learning.git Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE # Materials Application Domain (MAD)
 Research with respect to application domain with a materials science emphasis
```

### Comparing `madml-0.0.1/README.md` & `madml-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `madml-0.0.1/madml.egg-info/PKG-INFO` & `madml-0.0.2/madml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madml
-Version: 0.0.1
+Version: 0.0.2
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

 * *File "/tmp/diffoscope_h8o7bnlb_/tmp96vh1czb_TarContainer/0/5", line 99, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_h8o7bnlb_/tmp96vh1czb_TarContainer/0/5", line 99, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: madml Version: 0.0.1 Summary: Application domain of
+Metadata-Version: 2.1 Name: madml Version: 0.0.2 Summary: Application domain of
 machine learning in materials science. Home-page: https://github.com/leschultz/
 materials_application_domain_machine_learning.git Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE # Materials Application Domain (MAD)
 Research with respect to application domain with a materials science emphasis
```

### Comparing `madml-0.0.1/setup.py` & `madml-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 # Package information
 name = 'madml'
-version = '0.0.1'
+version = '0.0.2'
 description = 'Application domain of machine learning in materials science.'
 url = 'https://github.com/leschultz/'\
       'materials_application_domain_machine_learning.git'
 author = 'Lane E. Schultz'
 author_email = 'laneenriqueschultz@gmail.com'
 python_requires = '>=3.6'
 classifiers = ['Programming Language :: Python :: 3',
```

### Comparing `madml-0.0.1/tests/test_run.py` & `madml-0.0.2/tests/test_run.py`

 * *Files identical despite different names*

