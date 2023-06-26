# Comparing `tmp/plum_dispatch-2.1.0.tar.gz` & `tmp/plum_dispatch-2.1.1.tar.gz`

## Comparing `plum_dispatch-2.1.0.tar` & `plum_dispatch-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/_version.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/alias.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/autoreload.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/dispatcher.py
--rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/function.py
--rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/parametric.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/promotion.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/resolver.py
--rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/signature.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/type.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/plum/util.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/LICENCE.txt
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/README.md
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 plum_dispatch-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/_version.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/alias.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/autoreload.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/dispatcher.py
+-rw-r--r--   0        0        0    16829 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/function.py
+-rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/parametric.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/promotion.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/resolver.py
+-rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/signature.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/type.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/plum/util.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/LICENCE.txt
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 plum_dispatch-2.1.1/PKG-INFO
```

### Comparing `plum_dispatch-2.1.0/plum/__init__.py` & `plum_dispatch-2.1.1/plum/__init__.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/alias.py` & `plum_dispatch-2.1.1/plum/alias.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/autoreload.py` & `plum_dispatch-2.1.1/plum/autoreload.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/dispatcher.py` & `plum_dispatch-2.1.1/plum/dispatcher.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/function.py` & `plum_dispatch-2.1.1/plum/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,29 @@
     def __doc__(self):
         """str or None: Documentation of the function. This consists of the
         documentation of the function given at initialisation with the documentation
         of all other registered methods appended.
 
         Upon instantiation, this property is available through `obj.__doc__`.
         """
-        self._resolve_pending_registrations()
+        try:
+            self._resolve_pending_registrations()
+        except NameError:
+            # When `staticmethod` is combined with
+            # `from __future__ import annotations`, in Python 3.10 and higher
+            # `staticmethod` will attempt to inherit `__doc__` (see
+            # https://docs.python.org/3/library/functions.html#staticmethod). Since
+            # we are still in class construction, forward references are not yet
+            # defined, so attempting to resolve all pending methods might fail with a
+            # `NameError`. This is fine, because later calling `__doc__` on the
+            # `staticmethod` will again call this `__doc__`, at which point all methods
+            # will resolve properly. For now, we just ignore the error and undo the
+            # partially completed :meth:`Function._resolve_pending_registrations` by
+            # clearing the cache.
+            self.clear_cache(reregister=False)
 
         # Derive the basis of the docstring from `self._f`, removing any indentation.
         doc = self._doc.strip()
         if doc:
             # Do not include the first line when removing the indentation.
             lines = doc.splitlines()
             doc = lines[0]
```

### Comparing `plum_dispatch-2.1.0/plum/parametric.py` & `plum_dispatch-2.1.1/plum/parametric.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/promotion.py` & `plum_dispatch-2.1.1/plum/promotion.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/resolver.py` & `plum_dispatch-2.1.1/plum/resolver.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/signature.py` & `plum_dispatch-2.1.1/plum/signature.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/plum/type.py` & `plum_dispatch-2.1.1/plum/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import typing
 import warnings
 
 from .util import get_args, get_origin
 
 try:  # pragma: specific no cover 3.7 3.8 3.9
     from types import UnionType
-except ImportError:  # pragma: specific no cover 3.10
+except ImportError:  # pragma: specific no cover 3.10 3.11
 
     class UnionType:
         """Replacement for :class:`types.UnionType`."""
 
 
 try:  # pragma: specific no cover 3.7
     from typing import Literal
-except ImportError:  # pragma: specific no cover 3.8 3.9 3.10
+except ImportError:  # pragma: specific no cover 3.8 3.9 3.10 3.11
 
     class Literal:
         """A simple proxy for :class:`typing.Literal`."""
 
 
 __all__ = [
     "PromisedType",
@@ -192,15 +192,15 @@
                 return y
             else:
                 # Do not resolve the arguments for `Literal`s.
                 if origin != Literal:
                     args = resolve_type_hint(args)
                 try:
                     return origin[args]
-                except TypeError as e:  # pragma: specific no cover 3.9 3.10
+                except TypeError as e:  # pragma: specific no cover 3.9 3.10 3.11
                     # In Python 3.7 and 3.8, the origin might be a type that cannot be
                     # subscripted. As a workaround, we get the name of the type,
                     # capitalize it, and try to get it from `typing`. So far, this
                     # seems to have worked fine.
                     if sys.version_info.minor <= 8:
                         return getattr(typing, origin.__name__.capitalize())[args]
                     else:  # pragma: no cover
```

### Comparing `plum_dispatch-2.1.0/plum/util.py` & `plum_dispatch-2.1.1/plum/util.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/LICENCE.txt` & `plum_dispatch-2.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/README.md` & `plum_dispatch-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/pyproject.toml` & `plum_dispatch-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.1.0/PKG-INFO` & `plum_dispatch-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plum-dispatch
-Version: 2.1.0
+Version: 2.1.1
 Summary: Multiple dispatch in Python
 Project-URL: repository, https://github.com/beartype/plum
 Author-email: Wessel Bruinsma <wessel.p.bruinsma@gmail.com>
 License: MIT
 License-File: LICENCE.txt
 Keywords: multiple dispatch
 Classifier: Development Status :: 5 - Production/Stable
```

