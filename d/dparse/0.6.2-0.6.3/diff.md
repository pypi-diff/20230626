# Comparing `tmp/dparse-0.6.2.tar.gz` & `tmp/dparse-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dparse-0.6.2.tar", last modified: Mon Sep 19 20:38:11 2022, max compression
+gzip compressed data, was "dparse-0.6.3.tar", last modified: Mon Jun 26 15:38:24 2023, max compression
```

## Comparing `dparse-0.6.2.tar` & `dparse-0.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 20:38:11.193637 dparse-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-09-19 20:38:01.000000 dparse-0.6.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-09-19 20:38:01.000000 dparse-0.6.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-19 20:38:01.000000 dparse-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-09-19 20:38:01.000000 dparse-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7052 2022-09-19 20:38:11.193637 dparse-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-09-19 20:38:01.000000 dparse-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 20:38:11.193637 dparse-0.6.2/dparse/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    16396 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)     4708 2022-09-19 20:38:01.000000 dparse-0.6.2/dparse/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 20:38:11.193637 dparse-0.6.2/dparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7052 2022-09-19 20:38:11.000000 dparse-0.6.2/dparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-19 20:38:11.000000 dparse-0.6.2/dparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 20:38:11.000000 dparse-0.6.2/dparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 20:38:10.000000 dparse-0.6.2/dparse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-19 20:38:11.000000 dparse-0.6.2/dparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-19 20:38:11.000000 dparse-0.6.2/dparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 20:38:11.193637 dparse-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-19 20:38:01.000000 dparse-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 20:38:11.193637 dparse-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-19 20:38:01.000000 dparse-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-09-19 20:38:01.000000 dparse-0.6.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)    13264 2022-09-19 20:38:01.000000 dparse-0.6.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    16823 2022-09-19 20:38:01.000000 dparse-0.6.2/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 15:38:24.216697 dparse-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-06-26 15:38:13.000000 dparse-0.6.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-26 15:38:13.000000 dparse-0.6.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-26 15:38:13.000000 dparse-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-06-26 15:38:13.000000 dparse-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7251 2023-06-26 15:38:24.212697 dparse-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-06-26 15:38:13.000000 dparse-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 15:38:24.212697 dparse-0.6.3/dparse/
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6491 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16455 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/regex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-06-26 15:38:13.000000 dparse-0.6.3/dparse/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 15:38:24.212697 dparse-0.6.3/dparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7251 2023-06-26 15:38:24.000000 dparse-0.6.3/dparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-06-26 15:38:24.000000 dparse-0.6.3/dparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 15:38:24.000000 dparse-0.6.3/dparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 15:38:24.000000 dparse-0.6.3/dparse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-26 15:38:24.000000 dparse-0.6.3/dparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-26 15:38:24.000000 dparse-0.6.3/dparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 15:38:24.216697 dparse-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-26 15:38:13.000000 dparse-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 15:38:24.212697 dparse-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-26 15:38:13.000000 dparse-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-06-26 15:38:13.000000 dparse-0.6.3/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13264 2023-06-26 15:38:13.000000 dparse-0.6.3/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-06-26 15:38:13.000000 dparse-0.6.3/tests/test_updater.py
```

### Comparing `dparse-0.6.2/CONTRIBUTING.rst` & `dparse-0.6.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/HISTORY.rst` & `dparse-0.6.3/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+0.6.3 (2023-06-26)
+------------------
+
+* Use the modern tomli/tomllib to parse TOML files. (thanks @mgorny)
+* Drop Python 3.5 from our CI.
+
 0.6.2 (2022-09-19)
 ------------------
 
 * Fixed bug: always call the parent from the PATH in the resolve_file function.
 
 0.6.1 (2022-09-19)
 ------------------
```

### Comparing `dparse-0.6.2/LICENSE` & `dparse-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/PKG-INFO` & `dparse-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dparse
-Version: 0.6.2
+Version: 0.6.3
 Summary: A parser for Python dependency files
 Home-page: https://github.com/pyupio/dparse
 Author: Jannis Gebauer
 Author-email: support@pyup.io
 License: MIT license
 Keywords: dparse
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: pipenv
 Provides-Extra: conda
 License-File: LICENSE
 
 =================
 Dependency Parser
@@ -174,14 +175,20 @@
 environment to check the requirements file for your Python 2.7 project.
 
 
 =======
 History
 =======
 
+0.6.3 (2023-06-26)
+------------------
+
+* Use the modern tomli/tomllib to parse TOML files. (thanks @mgorny)
+* Drop Python 3.5 from our CI.
+
 0.6.2 (2022-09-19)
 ------------------
 
 * Fixed bug: always call the parent from the PATH in the resolve_file function.
 
 0.6.1 (2022-09-19)
 ------------------
```

### Comparing `dparse-0.6.2/README.rst` & `dparse-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/dparse/dependencies.py` & `dparse-0.6.3/dparse/dependencies.py`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/dparse/errors.py` & `dparse-0.6.3/dparse/errors.py`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/dparse/parser.py` & `dparse-0.6.3/dparse/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals, absolute_import
 
 import os
 from collections import OrderedDict
 import re
+import sys
 
 from io import StringIO
 
 from configparser import ConfigParser, NoOptionError
 from pathlib import PurePath
 
 from .errors import MalformedDependencyFileError
 from .regex import HASH_REGEX
 
 from .dependencies import DependencyFile, Dependency
 from packaging.requirements import Requirement as PackagingRequirement,\
     InvalidRequirement
 from . import filetypes
-import toml
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version, InvalidVersion
 import json
 
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
+
 
 # this is a backport from setuptools 26.1
 def setuptools_parse_requirements_backport(strs):  # pragma: no cover
     # Copyright (C) 2016 Jason R Coombs <jaraco@jaraco.com>
     #
     # Permission is hereby granted, free of charge, to any person obtaining a
     # copy of this software and associated documentation files
@@ -352,15 +357,15 @@
 
     def parse(self):
         """
         Parse a Pipfile (as seen in pipenv)
         :return:
         """
         try:
-            data = toml.loads(self.obj.content, _dict=OrderedDict)
+            data = tomllib.loads(self.obj.content)
             if data:
                 for package_type in ['packages', 'dev-packages']:
                     if package_type in data:
                         for name, specs in data[package_type].items():
                             # skip on VCS dependencies
                             if not isinstance(specs, str):
                                 continue
@@ -370,15 +375,15 @@
                                 Dependency(
                                     name=name, specs=SpecifierSet(specs),
                                     dependency_type=filetypes.pipfile,
                                     line=''.join([name, specs]),
                                     section=package_type
                                 )
                             )
-        except (toml.TomlDecodeError, IndexError):
+        except (tomllib.TOMLDecodeError, IndexError):
             pass
 
 
 class PipfileLockParser(Parser):
 
     def parse(self):
         """
@@ -439,15 +444,15 @@
 class PoetryLockParser(Parser):
 
     def parse(self):
         """
         Parse a poetry.lock
         """
         try:
-            data = toml.loads(self.obj.content, _dict=OrderedDict)
+            data = tomllib.loads(self.obj.content)
             pkg_key = 'package'
             if data:
                 try:
                     dependencies = data[pkg_key]
                 except KeyError:
                     raise KeyError(
                         "Poetry lock file is missing the package section")
@@ -467,15 +472,15 @@
                         Dependency(
                             name=name, specs=SpecifierSet(spec),
                             dependency_type=filetypes.poetry_lock,
                             line=''.join([name, spec]),
                             section=section
                         )
                     )
-        except (toml.TomlDecodeError, IndexError) as e:
+        except (tomllib.TOMLDecodeError, IndexError) as e:
             raise MalformedDependencyFileError(info=str(e))
 
 
 def parse(content, file_type=None, path=None, sha=None, marker=((), ()),
           parser=None, resolve=False):
     """
```

### Comparing `dparse-0.6.2/dparse/updater.py` & `dparse-0.6.3/dparse/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 import re
 import json
 import tempfile
-import toml
 import os
+import sys
+
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
 
 
 class RequirementsTXTUpdater(object):
     SUB_REGEX = r"^{}(?=\s*\r?\n?$)"
 
     @classmethod
     def update(cls, content, dependency, version, spec="==", hashes=()):
@@ -75,15 +80,15 @@
 class SetupCFGUpdater(CondaYMLUpdater):
     pass
 
 
 class PipfileUpdater(object):
     @classmethod
     def update(cls, content, dependency, version, spec="==", hashes=()):
-        data = toml.loads(content)
+        data = tomllib.loads(content)
         if data:
             for package_type in ['packages', 'dev-packages']:
                 if package_type in data:
                     if dependency.full_name in data[package_type]:
                         data[package_type][
                             dependency.full_name] = "{spec}{version}".format(
                             spec=spec, version=version
```

### Comparing `dparse-0.6.2/dparse.egg-info/PKG-INFO` & `dparse-0.6.3/dparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dparse
-Version: 0.6.2
+Version: 0.6.3
 Summary: A parser for Python dependency files
 Home-page: https://github.com/pyupio/dparse
 Author: Jannis Gebauer
 Author-email: support@pyup.io
 License: MIT license
 Keywords: dparse
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: pipenv
 Provides-Extra: conda
 License-File: LICENSE
 
 =================
 Dependency Parser
@@ -174,14 +175,20 @@
 environment to check the requirements file for your Python 2.7 project.
 
 
 =======
 History
 =======
 
+0.6.3 (2023-06-26)
+------------------
+
+* Use the modern tomli/tomllib to parse TOML files. (thanks @mgorny)
+* Drop Python 3.5 from our CI.
+
 0.6.2 (2022-09-19)
 ------------------
 
 * Fixed bug: always call the parent from the PATH in the resolve_file function.
 
 0.6.1 (2022-09-19)
 ------------------
```

### Comparing `dparse-0.6.2/setup.py` & `dparse-0.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,42 +9,43 @@
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
     "packaging",
-    "toml",
+    "tomli; python_version < '3.11'",
 ]
 
 setup(
     name='dparse',
-    version='0.6.2',
+    version='0.6.3',
     description="A parser for Python dependency files",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     author="Jannis Gebauer",
     author_email='support@pyup.io',
     url='https://github.com/pyupio/dparse',
     packages=find_packages(include=['dparse']),
     include_package_data=True,
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
     keywords='dparse',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
-    python_requires=">=3.5",
+    python_requires=">=3.6",
     extras_require={
-        'pipenv': ["pipenv"],
+        'pipenv': ["pipenv<=2022.12.19"],
         'conda': ["pyyaml"]
     }
 )
```

### Comparing `dparse-0.6.2/tests/test_dependencies.py` & `dparse-0.6.3/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/tests/test_parse.py` & `dparse-0.6.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dparse-0.6.2/tests/test_updater.py` & `dparse-0.6.3/tests/test_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,17 +451,11 @@
 django-allauth = "*"
 
 
 [dev-packages]
 
 toml = "*"
     """
-    import pipenv.project
-    monkeypatch.setattr(
-        pipenv.project.pipfile.Pipfile,
-        'find',
-        lambda max_depth: '/tmp/MockPipFile'
-    )
     dep_file = parse(content=content, file_type=filetypes.pipfile)
     dep = dep_file.dependencies[0]
     new_content = PipfileUpdater.update(content, version="2.1", dependency=dep)
     assert 'django = "==2.1"' in new_content
```

