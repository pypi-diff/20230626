# Comparing `tmp/pykebab-0.7.0.tar.gz` & `tmp/pykebab-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.7.0.tar", max compression
+gzip compressed data, was "pykebab-0.7.8.tar", max compression
```

## Comparing `pykebab-0.7.0.tar` & `pykebab-0.7.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.7.0/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.7.0/kebab/aws.py
--rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.7.0/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.7.0/kebab/cli/cli.py
--rw-r--r--   0        0        0      798 2023-02-03 08:02:22.409418 pykebab-0.7.0/kebab/constants.py
--rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.7.0/kebab/exceptions.py
--rw-r--r--   0        0        0     2587 2023-01-05 03:45:44.147717 pykebab-0.7.0/kebab/k8s.py
--rw-r--r--   0        0        0      773 2023-03-28 07:51:19.037015 pykebab-0.7.0/kebab/loader.py
--rw-r--r--   0        0        0     2381 2023-06-21 14:37:29.161728 pykebab-0.7.0/kebab/magic.py
--rw-r--r--   0        0        0     2108 2023-03-25 11:13:55.662982 pykebab-0.7.0/kebab/openers.py
--rw-r--r--   0        0        0    21897 2023-06-22 18:44:40.594527 pykebab-0.7.0/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.7.0/kebab/utils.py
--rw-r--r--   0        0        0     1025 2023-06-22 18:48:02.725805 pykebab-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/loader.py
+-rw-r--r--   0        0        0     2368 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/openers.py
+-rw-r--r--   0        0        0    22564 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-06-26 04:27:04.825862 pykebab-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.8/PKG-INFO
```

### Comparing `pykebab-0.7.0/kebab/__init__.py` & `pykebab-0.7.8/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/aws.py` & `pykebab-0.7.8/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/cli/cli.py` & `pykebab-0.7.8/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/constants.py` & `pykebab-0.7.8/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/k8s.py` & `pykebab-0.7.8/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/loader.py` & `pykebab-0.7.8/kebab/loader.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/magic.py` & `pykebab-0.7.8/kebab/magic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import time
-
 from kebab.sources import KebabSource, literal
 
 
 class Field:
     def __init__(
         self,
         config_name=None,
```

### Comparing `pykebab-0.7.0/kebab/openers.py` & `pykebab-0.7.8/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/kebab/sources.py` & `pykebab-0.7.8/kebab/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import dataclasses
 import logging
 import os
 import queue  # using python-future for 2/3 compatibility
 import threading
 import time
-from typing import Any, List, Dict, get_type_hints, Type, TypeVar
+from typing import Any, List, Dict, get_type_hints, Type, TypeVar, Callable
 from urllib.request import OpenerDirector
 
 import deprecation
 # noinspection PyPackageRequirements
 from pydantic import BaseModel
 
 from kebab.constants import DEFAULT_URL_ENVVAR, DISABLE_RELOAD
@@ -59,14 +59,15 @@
     def __init__(self, **kwargs):
         # Variables for sources reload (first load is also a reload).
         super(KebabSource, self).__init__(**kwargs)
         self._last_reload_timestamp = 0  # type: float
         self._reload_lock = threading.RLock()
         self._reload_timer = None
         self._reload_disabled = threading.Event()
+        self._last_cached_timestamp = 0  # type: float
         self._cached_context = {}
         self._str_loader = YamlLoader()
 
     def __repr__(self):
         return self.__class__.__name__
 
     def __getitem__(self, key):
@@ -171,23 +172,57 @@
                 )
                 self._reload_timer.daemon = True
                 self._reload_timer.start()
 
         return self
 
     def _get_context(self):
-        if not self._cached_context:
+        if (
+            not self._cached_context
+            or self._last_cached_timestamp < self.last_reload_timestamp
+        ):
             self.reload()
+            self._last_cached_timestamp = time.time()
 
         return self._cached_context
 
     @property
     def last_reload_timestamp(self):
         return self._last_reload_timestamp
 
+    T = TypeVar('T')
+
+    # noinspection PyMethodParameters
+    def proxy(source, f: Callable[[], T], expected_type: Type[T]) -> T:
+        if expected_type in (
+            int, str, float, bool, list, tuple, dict, set, type(None)
+        ):
+            return f()
+
+        # not thread safe
+        class KebabProxy:
+            def __init__(self):
+                self.__value = f()
+                self.__last_eval_timestamp = time.time()
+
+            def reload_if_necessary(self):
+                if self.__last_eval_timestamp < source.last_reload_timestamp:
+                    self.__value = f()
+                    self.__last_eval_timestamp = time.time()
+
+            def __getattr__(self, name):
+                self.reload_if_necessary()
+                ret = getattr(self.__value, name)
+
+                def reloader():
+                    self.reload_if_necessary()
+                    return getattr(self.__value, name)
+                return source.proxy(reloader, type(ret))
+        return KebabProxy()
+
     @deprecated_alias(default_value="default")
     def get(
         self,
         config_name=".",
         default=None,
         required=False,
         expected_type=None,
@@ -227,14 +262,24 @@
         Otherwise, it could return None.
 
         Note that the type of the default becomes the expected_type if presents,
         the original expected_type will be ignored in that case.
 
         The parameter `default_value` is deprecated, use `default` instead
         """
+        if update_after_reload:
+            # noinspection PyTypeChecker
+            return self.proxy(lambda: self.get(
+                config_name,
+                default,
+                required,
+                expected_type,
+                masked
+            ), expected_type=expected_type)
+
         if default is not None:
             # set expected type based on default value (and ignore the original
             # expected_type
             if expected_type is not None and not isinstance(default, expected_type):
                 raise ValueError(
                     "You specified default of type {}, but expected_type={}".format(
                         type(default), expected_type
@@ -258,36 +303,14 @@
                 raise KeyError(f"Missing value for {config_name}")
 
         config_value = self._cast(config_value, expected_type)
 
         printed_value = "*" * len(str(config_value)) if masked else config_value
         _logger.debug(f"read config: {config_name} = {printed_value}")
 
-        if update_after_reload:
-            class KebabProxy(expected_type):
-                def __init__(self2, value):
-                    self2._value = value
-                    self2._last_eval_timestamp = time.time()
-
-                def __getattr__(self2, name):
-                    # noinspection PyProtectedMember
-                    if (
-                        name != "_last_eval_timestamp"
-                        and self2._last_eval_timestamp < self.last_reload_timestamp
-                    ):
-                        self2._value = self.get(
-                            config_name=config_name,
-                            default=default,
-                            required=required,
-                            expected_type=expected_type,
-                            masked=masked)
-                        self._last_eval_timestamp = time.time()
-                    return getattr(self2._value, name)
-            return KebabProxy(config_value)
-
         return config_value
 
     @staticmethod
     def _cast_bool(config_value: Any) -> bool:
         if isinstance(config_value, str):
             v = config_value.lower()
             if v in ("1", "true", "yes", "on", "enable"):
@@ -336,16 +359,14 @@
                 elif dataclasses.is_dataclass(expected_type):
                     # noinspection PyTypeChecker
                     return KebabSource._to_dataclass(expected_type, config_value)
                 else:
                     return expected_type(config_value)
         return config_value
 
-    T = TypeVar('T')
-
     @staticmethod
     def _to_dataclass(data_class_type: Type[T], data: Dict[str, Any]) -> T:
         field_types = get_type_hints(data_class_type)
         return data_class_type(**{
             field: KebabSource._to_dataclass(field_types[field], data[field])
             if dataclasses.is_dataclass(field_types[field])
             else data[field]
@@ -540,14 +561,18 @@
         _context = {}
         for source in self._sources:
             next_context = source.reload()._get_context()
             _context = update_recursively(_context, next_context)
 
         return _context
 
+    @property
+    def last_reload_timestamp(self):
+        return max([s.last_reload_timestamp for s in self._sources])
+
 
 class SubSource(KebabSource):
     def __init__(self, parent_source, config_name, **kwargs):
         """
         Caveats:
 
         When parent KebabSource reloads, SubSource is not effected. In another word,
```

### Comparing `pykebab-0.7.0/kebab/utils.py` & `pykebab-0.7.8/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.0/pyproject.toml` & `pykebab-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.7.0"
+version = "0.7.8"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.7.0/PKG-INFO` & `pykebab-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.7.0
+Version: 0.7.8
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

