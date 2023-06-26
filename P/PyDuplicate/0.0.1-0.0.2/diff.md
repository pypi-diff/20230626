# Comparing `tmp/PyDuplicate-0.0.1.tar.gz` & `tmp/PyDuplicate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDuplicate-0.0.1.tar", last modified: Thu Jun 22 14:09:31 2023, max compression
+gzip compressed data, was "PyDuplicate-0.0.2.tar", last modified: Mon Jun 26 07:43:54 2023, max compression
```

## Comparing `PyDuplicate-0.0.1.tar` & `PyDuplicate-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 14:09:31.182653 PyDuplicate-0.0.1/
--rw-rw-rw-   0        0        0    35146 2023-05-23 08:15:10.000000 PyDuplicate-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3887 2023-06-22 14:09:31.181653 PyDuplicate-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 14:09:31.110255 PyDuplicate-0.0.1/PyDuplicate/
--rw-rw-rw-   0        0        0       51 2023-06-22 13:56:07.000000 PyDuplicate-0.0.1/PyDuplicate/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-22 13:37:03.000000 PyDuplicate-0.0.1/PyDuplicate/similarity.py
-drwxrwxrwx   0        0        0        0 2023-06-22 14:09:31.176609 PyDuplicate-0.0.1/PyDuplicate.egg-info/
--rw-rw-rw-   0        0        0     3887 2023-06-22 14:09:30.000000 PyDuplicate-0.0.1/PyDuplicate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-06-22 14:09:30.000000 PyDuplicate-0.0.1/PyDuplicate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 14:09:30.000000 PyDuplicate-0.0.1/PyDuplicate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-22 14:09:30.000000 PyDuplicate-0.0.1/PyDuplicate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 14:09:30.000000 PyDuplicate-0.0.1/PyDuplicate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3125 2023-06-22 13:47:15.000000 PyDuplicate-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 14:09:31.183652 PyDuplicate-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-06-22 13:27:16.000000 PyDuplicate-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:43:54.409168 PyDuplicate-0.0.2/
+-rw-rw-rw-   0        0        0    35146 2023-05-23 08:15:10.000000 PyDuplicate-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3887 2023-06-26 07:43:54.407168 PyDuplicate-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 07:43:54.356882 PyDuplicate-0.0.2/PyDuplicate/
+-rw-rw-rw-   0        0        0       51 2023-06-22 13:56:07.000000 PyDuplicate-0.0.2/PyDuplicate/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-22 13:37:03.000000 PyDuplicate-0.0.2/PyDuplicate/similarity.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:43:54.403993 PyDuplicate-0.0.2/PyDuplicate.egg-info/
+-rw-rw-rw-   0        0        0     3887 2023-06-26 07:43:54.000000 PyDuplicate-0.0.2/PyDuplicate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-26 07:43:54.000000 PyDuplicate-0.0.2/PyDuplicate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:43:54.000000 PyDuplicate-0.0.2/PyDuplicate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-26 07:43:54.000000 PyDuplicate-0.0.2/PyDuplicate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 07:43:54.000000 PyDuplicate-0.0.2/PyDuplicate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3125 2023-06-22 13:47:15.000000 PyDuplicate-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 07:43:54.409168 PyDuplicate-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-06-26 07:39:55.000000 PyDuplicate-0.0.2/setup.py
```

### Comparing `PyDuplicate-0.0.1/LICENSE` & `PyDuplicate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDuplicate-0.0.1/PKG-INFO` & `PyDuplicate-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDuplicate
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python functions for Efficient duplicate detection
 Home-page: https://github.com/JeanBertinR/PyDuplicate
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
 License: GPL-3.0
 Keywords: Duplicate detection,Efficient duplicate search
 Platform: UNKNOWN
```

### Comparing `PyDuplicate-0.0.1/PyDuplicate/similarity.py` & `PyDuplicate-0.0.2/PyDuplicate/similarity.py`

 * *Files identical despite different names*

### Comparing `PyDuplicate-0.0.1/PyDuplicate.egg-info/PKG-INFO` & `PyDuplicate-0.0.2/PyDuplicate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDuplicate
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python functions for Efficient duplicate detection
 Home-page: https://github.com/JeanBertinR/PyDuplicate
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
 License: GPL-3.0
 Keywords: Duplicate detection,Efficient duplicate search
 Platform: UNKNOWN
```

### Comparing `PyDuplicate-0.0.1/README.md` & `PyDuplicate-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyDuplicate-0.0.1/setup.py` & `PyDuplicate-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python functions for Efficient duplicate detection'
 LONG_DESCRIPTION = 'Provides efficient and intuitive functionality for detecting and removing duplicates within a given dataset'
 
 # Setting up
 setup(
     name="PyDuplicate",
     version=VERSION,
@@ -14,15 +14,15 @@
     author_email="<jeanbertin.ensam@gmail.com>",
     licence='GPL-3.0',
     description=DESCRIPTION,
     url="https://github.com/JeanBertinR/PyDuplicate",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=['re', 'difflib', 'fuzzywuzzy', 'numpy'],
+    install_requires=['difflib', 'fuzzywuzzy', 'numpy'],
     keywords=['Duplicate detection', 'Efficient duplicate search'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

