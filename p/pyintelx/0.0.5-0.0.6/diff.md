# Comparing `tmp/pyintelx-0.0.5.tar.gz` & `tmp/pyintelx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelx-0.0.5.tar", last modified: Mon Jun 26 19:17:51 2023, max compression
+gzip compressed data, was "pyintelx-0.0.6.tar", last modified: Mon Jun 26 19:28:26 2023, max compression
```

## Comparing `pyintelx-0.0.5.tar` & `pyintelx-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:51.269721 pyintelx-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 19:17:51.269721 pyintelx-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-26 19:17:40.000000 pyintelx-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:51.269721 pyintelx-0.0.5/pyintelx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:40.000000 pyintelx-0.0.5/pyintelx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:51.269721 pyintelx-0.0.5/pyintelx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-06-26 19:17:40.000000 pyintelx-0.0.5/pyintelx/cli/pyintelx
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 19:17:40.000000 pyintelx-0.0.5/pyintelx/intelx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:51.269721 pyintelx-0.0.5/pyintelx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 19:17:51.000000 pyintelx-0.0.5/pyintelx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 19:17:51.000000 pyintelx-0.0.5/pyintelx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:17:51.000000 pyintelx-0.0.5/pyintelx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:17:51.000000 pyintelx-0.0.5/pyintelx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:17:51.000000 pyintelx-0.0.5/pyintelx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:17:51.269721 pyintelx-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 19:17:40.000000 pyintelx-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 19:28:26.946318 pyintelx-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-26 19:28:17.000000 pyintelx-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/pyintelx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:17.000000 pyintelx-0.0.6/pyintelx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/pyintelx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-26 19:28:17.000000 pyintelx-0.0.6/pyintelx/cli/pyintelx
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 19:28:17.000000 pyintelx-0.0.6/pyintelx/intelx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/pyintelx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:28:26.946318 pyintelx-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 19:28:17.000000 pyintelx-0.0.6/setup.py
```

### Comparing `pyintelx-0.0.5/PKG-INFO` & `pyintelx-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.0.5
+Version: 0.0.6
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `pyintelx-0.0.5/README.md` & `pyintelx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyintelx-0.0.5/pyintelx/cli/pyintelx` & `pyintelx-0.0.6/pyintelx/cli/pyintelx`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import os
 import sys
 import html
 import json
 import time
 import tabulate
 import argparse
-from pyintelxio.intelx import intelx, IdentityService
-#from intelxapi import intelx, IdentityService
+from pyintelx import intelx,IdentityService
 from termcolor import colored
 from pygments import highlight
 from pygments.lexers import JsonLexer
 from pygments.formatters import TerminalFormatter
 
 BOLD = '\033[1m'
 END = '\033[0m'
```

### Comparing `pyintelx-0.0.5/pyintelx/intelx.py` & `pyintelx-0.0.6/pyintelx/intelx.py`

 * *Files identical despite different names*

### Comparing `pyintelx-0.0.5/pyintelx.egg-info/PKG-INFO` & `pyintelx-0.0.6/pyintelx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.0.5
+Version: 0.0.6
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `pyintelx-0.0.5/setup.py` & `pyintelx-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyintelx',
-    version='0.0.5',
+    version='0.0.6',
     description='This lib add support to use the Identity API from Intelx.io',
     install_requires=['requests'],
     license='MIT',
     keywords=['python, package, distribution'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Fermin Baudino, Einar Lanfranco',
```

