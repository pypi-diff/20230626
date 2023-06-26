# Comparing `tmp/pqdict-1.2.0.tar.gz` & `tmp/pqdict-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqdict-1.2.0.tar", last modified: Mon Nov 14 17:18:45 2022, max compression
+gzip compressed data, was "pqdict-1.2.1.tar", last modified: Mon Jun 26 20:08:13 2023, max compression
```

## Comparing `pqdict-1.2.0.tar` & `pqdict-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:18:45.702428 pqdict-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-11-14 17:18:31.000000 pqdict-1.2.0/CHANGES
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-11-14 17:18:31.000000 pqdict-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-14 17:18:31.000000 pqdict-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-11-14 17:18:45.702428 pqdict-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-11-14 17:18:31.000000 pqdict-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:18:45.698428 pqdict-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7409 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     9868 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)    62591 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/gillespie-output.png
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/pqdict.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-14 17:18:31.000000 pqdict-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:18:45.698428 pqdict-1.2.0/pqdict/
--rw-r--r--   0 runner    (1001) docker     (121)    19537 2022-11-14 17:18:31.000000 pqdict-1.2.0/pqdict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:18:45.702428 pqdict-1.2.0/pqdict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-11-14 17:18:45.000000 pqdict-1.2.0/pqdict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-11-14 17:18:45.000000 pqdict-1.2.0/pqdict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:18:45.000000 pqdict-1.2.0/pqdict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:18:45.000000 pqdict-1.2.0/pqdict.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-14 17:18:45.000000 pqdict-1.2.0/pqdict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-14 17:18:45.000000 pqdict-1.2.0/pqdict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-14 17:18:45.702428 pqdict-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-11-14 17:18:31.000000 pqdict-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:18:45.702428 pqdict-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    14721 2022-11-14 17:18:31.000000 pqdict-1.2.0/tests/test_pqdict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-26 20:08:03.000000 pqdict-1.2.1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-26 20:08:03.000000 pqdict-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 20:08:03.000000 pqdict-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 20:08:13.009665 pqdict-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 20:08:03.000000 pqdict-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.005665 pqdict-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    62591 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/gillespie-output.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/pqdict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/pqdict/
+-rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-06-26 20:08:03.000000 pqdict-1.2.1/pqdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-26 20:08:03.000000 pqdict-1.2.1/pqdict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:03.000000 pqdict-1.2.1/pqdict/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/pqdict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 20:08:13.000000 pqdict-1.2.1/pqdict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 20:08:13.009665 pqdict-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-26 20:08:03.000000 pqdict-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-26 20:08:03.000000 pqdict-1.2.1/tests/test_pqdict.py
```

### Comparing `pqdict-1.2.0/CHANGES` & `pqdict-1.2.1/CHANGES`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Release Notes
 =============
 
+1.2.1 (2023-06-26)
+++++++++++++++++++
+
+* Typing:
+	- Provided typing support (#19) applying stub generated by `@noamraph <https://github.com/noamraph>`_
+
+* Maintenance:
+	- Replaced CI badge.
+	- Dropped Python 2.7, no longer supported in CI. Next minor release will no longer support Python 2.
+
+
 1.2.0 (2022-10-14)
 ++++++++++++++++++
 
 * API changes:
 	- Added ``topvalue`` method (#17). By `@ShivKJ <https://github.com/ShivKJ>`_
 
 * Maintenance:
```

### Comparing `pqdict-1.2.0/LICENSE` & `pqdict-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.0/PKG-INFO` & `pqdict-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqdict
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Pythonic indexed priority queue
 Home-page: https://github.com/nvictus/priority-queue-dictionary
 Author: Nezar Abdennur
 Author-email: nabdennur@gmail.com
 License: MIT
 Keywords: dict,priority queue,heap,scheduler,data structures
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,17 +30,17 @@
 Priority Queue Dictionary (pqdict)
 ==================================
 
 A priority queue dictionary maps hashable objects (keys) to priority-determining values. It provides a hybrid dictionary/priority queue API. 
 
 Works with Python 2.7+, 3.4+, and PyPy.
 
-.. image:: https://travis-ci.org/nvictus/priority-queue-dictionary.png?branch=master   
-    :target: https://travis-ci.org/nvictus/priority-queue-dictionary
-    :alt: CI Build State
+.. image:: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml/badge.svg
+    :target: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml
+    :alt: CI
 
 .. image:: https://readthedocs.org/projects/pqdict/badge/?version=latest
     :target: https://readthedocs.org/projects/pqdict/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/pqdict.svg
     :target: https://pypi.python.org/pypi/pqdict
```

### Comparing `pqdict-1.2.0/README.rst` & `pqdict-1.2.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Priority Queue Dictionary (pqdict)
 ==================================
 
 A priority queue dictionary maps hashable objects (keys) to priority-determining values. It provides a hybrid dictionary/priority queue API. 
 
 Works with Python 2.7+, 3.4+, and PyPy.
 
-.. image:: https://travis-ci.org/nvictus/priority-queue-dictionary.png?branch=master   
-    :target: https://travis-ci.org/nvictus/priority-queue-dictionary
-    :alt: CI Build State
+.. image:: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml/badge.svg
+    :target: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml
+    :alt: CI
 
 .. image:: https://readthedocs.org/projects/pqdict/badge/?version=latest
     :target: https://readthedocs.org/projects/pqdict/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/pqdict.svg
     :target: https://pypi.python.org/pypi/pqdict
```

### Comparing `pqdict-1.2.0/docs/Makefile` & `pqdict-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.0/docs/conf.py` & `pqdict-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.0/docs/gillespie-output.png` & `pqdict-1.2.1/docs/gillespie-output.png`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.0/docs/intro.rst` & `pqdict-1.2.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.0/docs/pqdict.rst` & `pqdict-1.2.1/docs/pqdict.rst`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.0/docs/release.rst` & `pqdict-1.2.1/docs/release.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Release Notes
 =============
 
+1.2.1 (2023-06-26)
+++++++++++++++++++
+
+* Typing:
+	- Provided typing support (#19) applying stub generated by `@noamraph <https://github.com/noamraph>`_
+
+* Maintenance:
+	- Replaced CI badge.
+	- Dropped Python 2.7, no longer supported in CI. Next minor release will no longer support Python 2.
+
+
 1.2.0 (2022-10-14)
 ++++++++++++++++++
 
 * API changes:
 	- Added ``topvalue`` method (#17). By `@ShivKJ <https://github.com/ShivKJ>`_
 
 * Maintenance:
```

### Comparing `pqdict-1.2.0/pqdict/__init__.py` & `pqdict-1.2.1/pqdict/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 :license: MIT, see LICENSE for more details.
 
 """
 try:
     from collections.abc import MutableMapping as _MutableMapping
 except ImportError:
     # 2.7 compatability
-    from collections import MutableMapping as _MutableMapping
+    from collections import MutableMapping as _MutableMapping  # type: ignore
 
 from six.moves import range
 from operator import lt, gt
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __all__ = ["pqdict", "PQDict", "minpq", "maxpq", "nlargest", "nsmallest"]
 
 
 class _Node(object):
     __slots__ = ("key", "value", "prio")
 
     def __init__(self, key, value, prio):
@@ -60,15 +60,15 @@
         return self.__class__.__name__ + "(%s, %s, %s)" % (
             repr(self.key),
             repr(self.value),
             repr(self.prio),
         )
 
 
-class pqdict(_MutableMapping):
+class pqdict(_MutableMapping):  # pyright: ignore # Argument to class must be a base class (reportGeneralTypeIssues
     """
     A collection that maps hashable objects (keys) to priority-determining
     values. The mapping is mutable so items may be added, removed and have
     their priority level updated.
 
     Parameters
     ----------
```

### Comparing `pqdict-1.2.0/pqdict.egg-info/PKG-INFO` & `pqdict-1.2.1/pqdict.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqdict
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Pythonic indexed priority queue
 Home-page: https://github.com/nvictus/priority-queue-dictionary
 Author: Nezar Abdennur
 Author-email: nabdennur@gmail.com
 License: MIT
 Keywords: dict,priority queue,heap,scheduler,data structures
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,17 +30,17 @@
 Priority Queue Dictionary (pqdict)
 ==================================
 
 A priority queue dictionary maps hashable objects (keys) to priority-determining values. It provides a hybrid dictionary/priority queue API. 
 
 Works with Python 2.7+, 3.4+, and PyPy.
 
-.. image:: https://travis-ci.org/nvictus/priority-queue-dictionary.png?branch=master   
-    :target: https://travis-ci.org/nvictus/priority-queue-dictionary
-    :alt: CI Build State
+.. image:: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml/badge.svg
+    :target: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml
+    :alt: CI
 
 .. image:: https://readthedocs.org/projects/pqdict/badge/?version=latest
     :target: https://readthedocs.org/projects/pqdict/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/pqdict.svg
     :target: https://pypi.python.org/pypi/pqdict
```

### Comparing `pqdict-1.2.0/setup.py` & `pqdict-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,13 +58,16 @@
     description='A Pythonic indexed priority queue',
     long_description=get_long_description(),
     keywords=['dict', 'priority queue', 'heap', 'scheduler', 'data structures'],
     author='Nezar Abdennur',
     author_email='nabdennur@gmail.com',
     url='https://github.com/nvictus/priority-queue-dictionary',
     packages=['pqdict'],
+    package_data={
+        'pqdict': ['py.typed', '*.pyi'],
+    },
     zip_safe=False,
     classifiers=[s.strip() for s in classifiers.split('\n') if s],
     install_requires=['six'],
     tests_require=['pytest'],
     extras_require={'docs': ['Sphinx>=1.1', 'numpydoc']},
 )
```

### Comparing `pqdict-1.2.0/tests/test_pqdict.py` & `pqdict-1.2.1/tests/test_pqdict.py`

 * *Files identical despite different names*

