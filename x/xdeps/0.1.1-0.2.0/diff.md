# Comparing `tmp/xdeps-0.1.1.tar.gz` & `tmp/xdeps-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdeps-0.1.1.tar", last modified: Tue Jun  6 14:39:39 2023, max compression
+gzip compressed data, was "xdeps-0.2.0.tar", last modified: Mon Jun 26 16:13:31 2023, max compression
```

## Comparing `xdeps-0.1.1.tar` & `xdeps-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.243203 xdeps-0.1.1/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.1.1/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-06 14:39:39.243002 xdeps-0.1.1/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-06-06 14:39:39.243276 xdeps-0.1.1/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.1.1/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.234983 xdeps-0.1.1/xdeps/
--rw-r--r--   0 giadarol   (503) staff       (20)      416 2023-06-06 14:39:09.000000 xdeps-0.1.1/xdeps/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-06 14:39:22.000000 xdeps-0.1.1/xdeps/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.1.1/xdeps/madxutils.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.242693 xdeps-0.1.1/xdeps/optimize/
--rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/optimize/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3511 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/optimize/jacobian.py
--rw-r--r--   0 giadarol   (503) staff       (20)    11173 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/optimize/optimize.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21520 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/refs.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.1.1/xdeps/sorting.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16572 2023-06-06 14:39:09.000000 xdeps-0.1.1/xdeps/table.py
--rw-r--r--   0 giadarol   (503) staff       (20)    14604 2023-05-23 20:23:29.000000 xdeps-0.1.1/xdeps/tasks.py
--rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.1.1/xdeps/utils.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.241591 xdeps-0.1.1/xdeps.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      389 2023-06-06 14:39:39.000000 xdeps-0.1.1/xdeps.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.411731 xdeps-0.2.0/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.2.0/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-26 16:13:31.411519 xdeps-0.2.0/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-06-26 16:13:31.411786 xdeps-0.2.0/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.2.0/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.403930 xdeps-0.2.0/xdeps/
+-rw-r--r--   0 giadarol   (503) staff       (20)      462 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-26 16:12:56.000000 xdeps-0.2.0/xdeps/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      397 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/functions.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.2.0/xdeps/madxutils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.411055 xdeps-0.2.0/xdeps/optimize/
+-rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/optimize/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3511 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/optimize/jacobian.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    11173 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/optimize/optimize.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    22746 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/refs.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.2.0/xdeps/sorting.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16572 2023-06-06 14:39:09.000000 xdeps-0.2.0/xdeps/table.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    15105 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/tasks.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.2.0/xdeps/utils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.407640 xdeps-0.2.0/xdeps.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      408 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/top_level.txt
```

### Comparing `xdeps-0.1.1/LICENSE` & `xdeps-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/PKG-INFO` & `xdeps-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.1.1
+Version: 0.2.0
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xdeps-0.1.1/setup.py` & `xdeps-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps/madxutils.py` & `xdeps-0.2.0/xdeps/madxutils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps/optimize/jacobian.py` & `xdeps-0.2.0/xdeps/optimize/jacobian.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps/optimize/optimize.py` & `xdeps-0.2.0/xdeps/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps/refs.py` & `xdeps-0.2.0/xdeps/refs.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         newexpr=self._expr
         if newexpr:
             return newexpr{sy}other
         else:
             return self._get_value(){sy}other"""
         print(fmt)
 
+def _isref(obj):
+    return isinstance(obj, ARef)
 
 class ARef:
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
         raise ValueError("Cannot instantiate ARef")
 
@@ -775,14 +777,60 @@
         if isinstance(self._func, ARef):
             fname = repr(self._func)
         else:
             fname = self._func.__name__
         return f"{fname}({args})"
 
 
+class RefList:
+    """
+    A list implementation that does not use __eq__ for comparisons. It is used
+    for storing tasks, which need to be compared by their hash, as the usual
+    == operator yields an expression, which is always True.
+    """
+    def __init__(self, *args, **kwargs):
+        self.list = list(*args, **kwargs)
+
+    def __repr__(self):
+        return f"RefList({self.list})"
+
+    def __contains__(self, item):
+        try:
+            self.index(item)
+            return True
+        except ValueError:
+            return False
+
+    def __getitem__(self, item):
+        return self.list[item]
+
+    def __delitem__(self, index):
+        self.list.pop(index)
+
+    def __iter__(self):
+        return iter(self.list)
+
+    def index(self, item):
+        for ii, x in enumerate(self.list):
+            if hash(item) == hash(x):
+                return ii
+        raise ValueError(f'{item} is not in list')
+
+    def extend(self, other):
+        if isinstance(other, RefList):
+            other = other.list
+        self.list.extend(other)
+
+    def append(self, item):
+        self.list.append(item)
+
+    def remove(self, item):
+        del self[self.index(item)]
+
+
 gbl = globals()
 for st, op in _binops.items():
     fn = op.__name__.replace("_", "")
     cn = f"{fn.capitalize()}Ref"
     mn = f"__{fn}__"
     gbl[cn] = type(cn, (BinOpRef,), {"_op": op, "_st": st})
```

### Comparing `xdeps-0.1.1/xdeps/sorting.py` & `xdeps-0.2.0/xdeps/sorting.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps/table.py` & `xdeps-0.2.0/xdeps/table.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps/tasks.py` & `xdeps-0.2.0/xdeps/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 # ######################################### #
 
 from dataclasses import dataclass, field
 from collections import defaultdict
 import logging
 from copy import deepcopy
 
-from .refs import ARef, Ref, ObjectAttrRef
-from .refs import AttrRef, CallRef, ItemRef
+from .refs import ARef, CallRef, Ref, ObjectAttrRef, RefList
 from .utils import os_display_png, mpl_display_png, ipy_display_png
 from .utils import AttrDict
 from .sorting import toposort
 
 logger = logging.getLogger(__name__)
 
 
@@ -125,27 +124,28 @@
 
 class Manager:
     """
     Value dependency manager:
 
     tasks: taskid -> task
     rdeps: ref -> set of all refs that depends on `ref`
-    rtasks: taskid -> set all tasks whose dependencies are affected by taskid
+    rtasks: taskid -> all tasks whose dependencies are affected by taskid
     deptasks: ref -> all tasks that has ref as dependency
     tartasks: ref -> all tasks that has ref as target
     containers: label -> controlled container
     """
 
     def __init__(self):
         self.tasks = {}
         self.containers = {}
-        self.rdeps = defaultdict(list)
-        self.rtasks = defaultdict(list)
-        self.deptasks = defaultdict(list)
-        self.tartasks = defaultdict(list)
+        self.rdeps = defaultdict(RefList)
+        self.rtasks = defaultdict(RefList)
+        self.deptasks = defaultdict(RefList)
+        self.tartasks = defaultdict(RefList)
+        self._tree_frozen = False
 
     def ref(self, container=None, label="_"):
         """Return a ref to an instance (or dict) associated to a label.
 
         Label must be unique.
         """
         if container is None:
@@ -173,14 +173,18 @@
         for task in tasks:
             logger.info("Run %s", task)
             task.run()
 
     def register(self, task):
         """Register a new task identified by taskid"""
         # logger.info("register %s",taskid)
+        if self._tree_frozen:
+            raise ValueError("Expressions and references cannot be changed "
+                             "because the tree is frozen (e.g. because "
+                             "a variables cache is active)")
         taskid = task.taskid
         self.tasks[taskid] = task
         for dep in task.dependencies:
             # logger.info("%s have an impact on %s",dep,task.targets)
             self.rdeps[dep].extend(task.targets)
             # logger.info("%s is used by T:%s",dep,taskid)
             self.deptasks[dep].append(taskid)
@@ -192,20 +196,24 @@
             self.tartasks[tar].append(taskid)
             for deptask in self.deptasks[tar]:
                 # logger.info("T:%s modifies deps of T:%s",taskid,deptask)
                 self.rtasks[taskid].append(deptask)
 
     def unregister(self, taskid):
         """Unregister the task identified by taskid"""
+        if self._tree_frozen:
+            raise ValueError("Expressions and references cannot be changed "
+                             "because the tree is frozen (e.g. because "
+                             "a variables cache is active)")
         task = self.tasks[taskid]
         for dep in task.dependencies:
             for target in task.targets:
                 if target in self.rdeps[dep]:
                     self.rdeps[dep].remove(target)
-            if dep in self.rtasks[dep]:
+            if taskid in self.rtasks[dep]:
                 self.rtasks[dep].remove(taskid)
             if taskid in self.deptasks[dep]:
                 self.deptasks[dep].remove(taskid)
         for tar in task.targets:
             self.tartasks[tar].remove(taskid)
             for deptask in self.deptasks[tar]:
                 if taskid in self.rtasks[deptask]:
```

### Comparing `xdeps-0.1.1/xdeps/utils.py` & `xdeps-0.2.0/xdeps/utils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.1/xdeps.egg-info/PKG-INFO` & `xdeps-0.2.0/xdeps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.1.1
+Version: 0.2.0
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

