# Comparing `tmp/flake8-isolated-packages-2.1.0.tar.gz` & `tmp/flake8_isolated_packages-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-isolated-packages-2.1.0.tar", last modified: Wed Jun 21 08:57:17 2023, max compression
+gzip compressed data, was "flake8_isolated_packages-2.2.0.tar", max compression
```

## Comparing `flake8-isolated-packages-2.1.0.tar` & `flake8_isolated_packages-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxr-xr-x   0 d.dudov    (502) staff       (20)        0 2023-06-21 08:57:17.477563 flake8-isolated-packages-2.1.0/
--rw-r--r--   0 d.dudov    (502) staff       (20)     1070 2021-02-27 13:16:03.000000 flake8-isolated-packages-2.1.0/LICENSE
--rw-r--r--   0 d.dudov    (502) staff       (20)     1805 2023-06-21 08:57:17.477706 flake8-isolated-packages-2.1.0/PKG-INFO
--rw-r--r--   0 d.dudov    (502) staff       (20)      892 2021-03-02 11:27:51.000000 flake8-isolated-packages-2.1.0/README.md
-drwxr-xr-x   0 d.dudov    (502) staff       (20)        0 2023-06-21 08:57:17.477154 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/
--rw-r--r--   0 d.dudov    (502) staff       (20)     1805 2023-06-21 08:57:16.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/PKG-INFO
--rw-r--r--   0 d.dudov    (502) staff       (20)      369 2023-06-21 08:57:17.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/SOURCES.txt
--rw-r--r--   0 d.dudov    (502) staff       (20)        1 2023-06-21 08:57:16.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/dependency_links.txt
--rw-r--r--   0 d.dudov    (502) staff       (20)       57 2023-06-21 08:57:17.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/entry_points.txt
--rw-r--r--   0 d.dudov    (502) staff       (20)       36 2023-06-21 08:57:17.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/requires.txt
--rw-r--r--   0 d.dudov    (502) staff       (20)       26 2023-06-21 08:57:17.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/top_level.txt
--rw-r--r--   0 d.dudov    (502) staff       (20)     3421 2022-06-08 11:07:54.000000 flake8-isolated-packages-2.1.0/flake8_isolated_packages.py
--rw-r--r--   0 d.dudov    (502) staff       (20)      666 2023-06-21 08:53:29.000000 flake8-isolated-packages-2.1.0/pyproject.toml
--rw-r--r--   0 d.dudov    (502) staff       (20)      435 2023-06-21 08:57:17.478451 flake8-isolated-packages-2.1.0/setup.cfg
--rw-r--r--   0 d.dudov    (502) staff       (20)     1296 2023-06-21 08:56:35.000000 flake8-isolated-packages-2.1.0/setup.py
+-rw-r--r--   0        0        0     1070 2021-02-27 13:16:03.301056 flake8_isolated_packages-2.2.0/LICENSE
+-rw-r--r--   0        0        0      892 2021-03-02 11:27:51.305414 flake8_isolated_packages-2.2.0/README.md
+-rw-r--r--   0        0        0     3421 2022-06-08 11:07:54.945300 flake8_isolated_packages-2.2.0/flake8_isolated_packages.py
+-rw-r--r--   0        0        0      666 2023-06-26 13:36:13.553271 flake8_isolated_packages-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1715 2023-06-26 13:38:51.170786 flake8_isolated_packages-2.2.0/setup.py
+-rw-r--r--   0        0        0     1689 2023-06-26 13:38:51.171043 flake8_isolated_packages-2.2.0/PKG-INFO
```

### Comparing `flake8-isolated-packages-2.1.0/LICENSE` & `flake8_isolated_packages-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-isolated-packages-2.1.0/PKG-INFO` & `flake8_isolated_packages-2.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: flake8-isolated-packages
-Version: 2.1.0
-Summary: This flake8 plugin is for checking imports isolations.
+Version: 2.2.0
+Summary: This Flake8 plugin is for checking imports isolations.
 Home-page: https://github.com/DDmitiy/flake8_isolated_packages
-Author: Dudov Dmitriy (ddmitiy)
-Author-email: dudov.dm@gmail.com
 License: MIT
-Keywords: flake8,plugin,imports,packages,isolation
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
+Keywords: flake8_isolated_packages,flake8,plugin,isolated_packages
+Author: Dudov Dmitry
+Author-email: dudov.dm@gmail.com
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: astpretty (>=2.1.0,<3.0.0)
+Requires-Dist: flake8 (>=3.0)
+Project-URL: Repository, https://github.com/DDmitiy/flake8_isolated_packages
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # flake8_isolated_packages
 
 This *Flake8* plugin is for checking imports isolations.  
 **One rule:** Any module from specified package could not be import in another package
 
 # Quick Start Guide
@@ -55,8 +52,7 @@
 
 **isolated_packages**  
 It specifies a list of folders, that cannot be imported outside of their package
 
 **test_folders**  
 It specifies a list of folders, that contains tests and in which can be imported something from even isolated packages
 
-
```

### Comparing `flake8-isolated-packages-2.1.0/README.md` & `flake8_isolated_packages-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8-isolated-packages-2.1.0/flake8_isolated_packages.egg-info/PKG-INFO` & `flake8_isolated_packages-2.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: flake8-isolated-packages
-Version: 2.1.0
-Summary: This flake8 plugin is for checking imports isolations.
-Home-page: https://github.com/DDmitiy/flake8_isolated_packages
-Author: Dudov Dmitriy (ddmitiy)
-Author-email: dudov.dm@gmail.com
-License: MIT
-Keywords: flake8,plugin,imports,packages,isolation
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-# flake8_isolated_packages
-
-This *Flake8* plugin is for checking imports isolations.  
-**One rule:** Any module from specified package could not be import in another package
-
-# Quick Start Guide
-
-1. Install ``flake8-isolated-packages`` from PyPI with pip::
-
-        pip install flake8-isolated-packages
-
-2. Configure a mark that you would like to validate::
-
-        cd project_root/
-        vi setup.cfg
-
-3. Add to file following: 
-   
-        [flake8]  
-        isolated_packages = service, tests  
-        test_folders = tests
-
-3. Run flake8::
-
-        flake8 .
-
-# flake8 codes
-
-   * FIP100: You try to import from isolated package
-
-# Settings
-
-**isolated_packages**  
-It specifies a list of folders, that cannot be imported outside of their package
-
-**test_folders**  
-It specifies a list of folders, that contains tests and in which can be imported something from even isolated packages
+modules = \
+['flake8_isolated_packages']
+install_requires = \
+['astpretty>=2.1.0,<3.0.0', 'flake8>=3.0']
+
+entry_points = \
+{'flake8.extension': ['FIP = flake8_isolated_packages:Plugin']}
+
+setup_kwargs = {
+    'name': 'flake8-isolated-packages',
+    'version': '2.2.0',
+    'description': 'This Flake8 plugin is for checking imports isolations.',
+    'long_description': '# flake8_isolated_packages\n\nThis *Flake8* plugin is for checking imports isolations.  \n**One rule:** Any module from specified package could not be import in another package\n\n# Quick Start Guide\n\n1. Install ``flake8-isolated-packages`` from PyPI with pip::\n\n        pip install flake8-isolated-packages\n\n2. Configure a mark that you would like to validate::\n\n        cd project_root/\n        vi setup.cfg\n\n3. Add to file following: \n   \n        [flake8]  \n        isolated_packages = service, tests  \n        test_folders = tests\n\n3. Run flake8::\n\n        flake8 .\n\n# flake8 codes\n\n   * FIP100: You try to import from isolated package\n\n# Settings\n\n**isolated_packages**  \nIt specifies a list of folders, that cannot be imported outside of their package\n\n**test_folders**  \nIt specifies a list of folders, that contains tests and in which can be imported something from even isolated packages\n',
+    'author': 'Dudov Dmitry',
+    'author_email': 'dudov.dm@gmail.com',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': 'https://github.com/DDmitiy/flake8_isolated_packages',
+    'py_modules': modules,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
+    'python_requires': '>=3.7,<4.0',
+}
 
 
+setup(**setup_kwargs)
```

### Comparing `flake8-isolated-packages-2.1.0/flake8_isolated_packages.py` & `flake8_isolated_packages-2.2.0/flake8_isolated_packages.py`

 * *Files identical despite different names*

### Comparing `flake8-isolated-packages-2.1.0/pyproject.toml` & `flake8_isolated_packages-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8_isolated_packages"
-version = "2.1.0"
+version = "2.2.0"
 description = "This Flake8 plugin is for checking imports isolations."
 authors = ["Dudov Dmitry <dudov.dm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DDmitiy/flake8_isolated_packages"
 repository = "https://github.com/DDmitiy/flake8_isolated_packages"
 keywords = ["flake8_isolated_packages", "flake8", "plugin", "isolated_packages"]
```

