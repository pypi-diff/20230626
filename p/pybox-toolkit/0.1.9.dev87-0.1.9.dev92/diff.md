# Comparing `tmp/pybox-toolkit-0.1.9.dev87.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.9.dev87.tar", last modified: Sun Jun 25 10:56:39 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev92.tar", last modified: Sat Jun 24 17:24:57 2023, max compression
```

## Comparing `pybox-toolkit-0.1.9.dev87.tar` & `pybox-toolkit-0.1.9.dev92.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev87/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev87/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.313406 pybox-toolkit-0.1.9.dev87/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.317406 pybox-toolkit-0.1.9.dev87/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-25 10:56:39.000000 pybox-toolkit-0.1.9.dev87/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-25 10:56:39.000000 pybox-toolkit-0.1.9.dev87/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 10:56:39.000000 pybox-toolkit-0.1.9.dev87/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-25 10:56:39.000000 pybox-toolkit-0.1.9.dev87/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-25 10:56:39.000000 pybox-toolkit-0.1.9.dev87/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15551 2023-06-25 10:54:45.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/graphing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 10:56:00.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5185 2023-06-25 10:54:45.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 10:56:39.321406 pybox-toolkit-0.1.9.dev87/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev87/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.404097 pybox-toolkit-0.1.9.dev92/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/graphing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-24 17:24:33.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5185 2023-06-24 15:29:00.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-05 19:32:07.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-31 11:15:50.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.9.dev87/pyproject.toml` & `pybox-toolkit-0.1.9.dev92/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev87/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 
 import mpmath
 import sympy
 from sympy.core.basic import Basic as SympyBasic
 
 from toolkit import test
 from toolkit.typing import BaseUnit, Unit, _UnitClassParser
-from toolkit.utils import (ArgumentException, DocumentationException,
-                           RangeException, RuntimeException, TestingException,
-                           map_dictionary_key, map_dictionary_value)
+from toolkit.utils import (
+    ArgumentException,
+    DocumentationException,
+    RangeException,
+    RuntimeException,
+    TestingException,
+    map_dictionary_key,
+    map_dictionary_value,
+)
 
 
 class BaseFormula:
     """
     Contains information about a formula, including:
             - Parameter ranges
             - Labels
@@ -399,9 +405,7 @@
     Args:
         func (Optional[Callable[..., Union[Unit, tuple[Unit, ...]]]], optional): Function implementation. Default: None.
 
     Returns:
         __ImpureFormula: The formula object.
     """
     return __formula(_ImpureFormula, func, **kwargs)
-
-# This comment is a hack to get the pipeline to pass the day of the deadline. Please remove some day :)
```

### Comparing `pybox-toolkit-0.1.9.dev87/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev87/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev87/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev87/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev87/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/utils.py`

 * *Files identical despite different names*

