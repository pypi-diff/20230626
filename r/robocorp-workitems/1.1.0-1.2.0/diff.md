# Comparing `tmp/robocorp_workitems-1.1.0.tar.gz` & `tmp/robocorp_workitems-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_workitems-1.1.0.tar", max compression
+gzip compressed data, was "robocorp_workitems-1.2.0.tar", max compression
```

## Comparing `robocorp_workitems-1.1.0.tar` & `robocorp_workitems-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5629 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/README.md
--rw-r--r--   0        0        0      817 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4980 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/__init__.py
--rw-r--r--   0        0        0    17330 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_adapters.py
--rw-r--r--   0        0        0     2380 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_context.py
--rw-r--r--   0        0        0      958 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_exceptions.py
--rw-r--r--   0        0        0     6520 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_requests.py
--rw-r--r--   0        0        0     1657 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_types.py
--rw-r--r--   0        0        0     2331 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_utils.py
--rw-r--r--   0        0        0     8789 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_workitem.py
--rw-r--r--   0        0        0        0 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/py.typed
--rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 robocorp_workitems-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5629 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/README.md
+-rw-r--r--   0        0        0      889 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4839 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/__init__.py
+-rw-r--r--   0        0        0    17330 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_adapters.py
+-rw-r--r--   0        0        0     2380 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_context.py
+-rw-r--r--   0        0        0      958 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_exceptions.py
+-rw-r--r--   0        0        0     6520 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_requests.py
+-rw-r--r--   0        0        0     1613 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_types.py
+-rw-r--r--   0        0        0     2401 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_utils.py
+-rw-r--r--   0        0        0     8789 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/_workitem.py
+-rw-r--r--   0        0        0        0 2023-06-26 08:04:35.424126 robocorp_workitems-1.2.0/src/robocorp/workitems/py.typed
+-rw-r--r--   0        0        0     6452 1970-01-01 00:00:00.000000 robocorp_workitems-1.2.0/PKG-INFO
```

### Comparing `robocorp_workitems-1.1.0/README.md` & `robocorp_workitems-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.1.0/pyproject.toml` & `robocorp_workitems-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [tool.poetry]
 name = "robocorp-workitems"
-version = "1.1.0"
+version = "1.2.0"
 description = "Robocorp Work Items library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
+repository = "https://github.com/robocorp/robo/"
+license = "Apache-2.0"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.black]
 skip-string-normalization = false
 skip-magic-trailing-comma = false
 
 [tool.isort]
```

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/__init__.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
 from typing import Callable, Optional, Union, cast
 
 from robocorp.tasks import get_current_task, task_cache
 
+from ._adapters import BaseAdapter, FileAdapter, RobocorpAdapter
 from ._context import Context
 from ._exceptions import (
     ApplicationException,
     BusinessException,
     EmptyQueue,
     to_exception_type,
 )
 from ._types import ExceptionType, JSONType, State
 from ._workitem import Input, Output
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
 @task_cache
 def __ctx():
@@ -62,20 +63,14 @@
 
 
 class Inputs:
     """Inputs represents the input queue of work items.
 
     It can be used to reserve and release items from the queue,
     and iterate over them.
-
-    Example:
-        Multiple items can behandled by iterating over this class::
-
-            for item in inputs:
-                handle_item(item.payload)
     """
 
     def __iter__(self):
         if self.current and not self.current.released:
             with self.current as item:
                 yield item
 
@@ -113,19 +108,14 @@
         return _ctx().reserve_input()
 
 
 class Outputs:
     """Outputs represents the output queue of work items.
 
     It can be used to create outputs and inspect the items created during the execution.
-
-    Example:
-        The class can be used to create outputs::
-
-            outputs.create({"key": "value"})
     """
 
     def __len__(self):
         return len(_ctx().outputs)
 
     def __getitem__(self, key):
         return _ctx().outputs[key]
@@ -181,14 +171,17 @@
         return item
 
 
 inputs = Inputs()
 outputs = Outputs()
 
 __all__ = [
+    "BaseAdapter",
+    "FileAdapter",
+    "RobocorpAdapter",
     "EmptyQueue",
     "BusinessException",
     "ApplicationException",
     "State",
     "ExceptionType",
     "Input",
     "Output",
```

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/_adapters.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/_adapters.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/_context.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/_exceptions.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/_requests.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/_utils.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             pass
 
     raise ValueError(f"No module/attribute with name: {name}")
 
 
 def resolve_path(path: str) -> Path:
     """Resolve a string-based path, and replace variables."""
+    # TODO: Support RF syntax for replacement, such as ${ROBOT_ROOT}?
     return Path(path).expanduser().resolve()
 
 
 def url_join(*parts):
     """Join parts of URL and handle missing/duplicate slashes."""
     return "/".join(str(part).strip("/") for part in parts)
```

### Comparing `robocorp_workitems-1.1.0/src/robocorp/workitems/_workitem.py` & `robocorp_workitems-1.2.0/src/robocorp/workitems/_workitem.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.1.0/PKG-INFO` & `robocorp_workitems-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: robocorp-workitems
-Version: 1.1.0
+Version: 1.2.0
 Summary: Robocorp Work Items library
+Home-page: https://github.com/robocorp/robo/
+License: Apache-2.0
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: robocorp-tasks (>=1,<2)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # robocorp-workitems
 
 Work items are used in Robocorp Control Room for managing data that go through
 multiple steps and tasks inside a process. Each step of a process receives input
 work items from the previous step, and creates output work items for the next
```

