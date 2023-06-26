# Comparing `tmp/pykebab-0.7.4.tar.gz` & `tmp/pykebab-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.7.4.tar", max compression
+gzip compressed data, was "pykebab-0.7.5.tar", max compression
```

## Comparing `pykebab-0.7.4.tar` & `pykebab-0.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/cli/cli.py
--rw-r--r--   0        0        0      798 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/exceptions.py
--rw-r--r--   0        0        0     2587 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/k8s.py
--rw-r--r--   0        0        0      773 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/loader.py
--rw-r--r--   0        0        0     2368 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/magic.py
--rw-r--r--   0        0        0     2108 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/openers.py
--rw-r--r--   0        0        0    21801 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-06-25 18:26:03.118172 pykebab-0.7.4/kebab/utils.py
--rw-r--r--   0        0        0     1025 2023-06-25 18:26:03.118172 pykebab-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/loader.py
+-rw-r--r--   0        0        0     2368 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/openers.py
+-rw-r--r--   0        0        0    22493 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-06-26 02:41:43.372858 pykebab-0.7.5/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-06-26 02:41:43.376858 pykebab-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.5/PKG-INFO
```

### Comparing `pykebab-0.7.4/kebab/__init__.py` & `pykebab-0.7.5/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/aws.py` & `pykebab-0.7.5/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/cli/cli.py` & `pykebab-0.7.5/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/constants.py` & `pykebab-0.7.5/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/k8s.py` & `pykebab-0.7.5/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/loader.py` & `pykebab-0.7.5/kebab/loader.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/magic.py` & `pykebab-0.7.5/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/openers.py` & `pykebab-0.7.5/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/kebab/sources.py` & `pykebab-0.7.5/kebab/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,15 @@
             try:
                 _context = self._load_context_recursively()
 
                 # lock only when switch
                 with self._reload_lock:
                     self._cached_context = _context
                     self._last_reload_timestamp = time.time()
+                    print(f"source reloading {self._last_reload_timestamp}")
             except Exception as e:
                 _logger.warning(
                     f"failed to reload, will use the cached value for {self}\n {e}"
                 )
 
         # reload periodically if reload_interval_in_secs > 0
         if reload_interval_in_secs > 0:
@@ -183,26 +184,43 @@
     @property
     def last_reload_timestamp(self):
         return self._last_reload_timestamp
 
     T = TypeVar('T')
 
     # noinspection PyMethodParameters
-    def proxy(source, f: Callable[[], T]) -> T:
+    def proxy(source, f: Callable[[], T], expected_type: Type[T]) -> T:
+        if expected_type in (
+            int, str, float, bool, type(None)
+        ):
+            return f()
+
         # not thread safe
         class KebabProxy:
             def __init__(self):
                 self.__value = f()
                 self.__last_eval_timestamp = time.time()
 
-            def __getattr__(self, name):
+            def reload(self):
+                print(f"proxy compare {self.__last_eval_timestamp} {source.last_reload_timestamp}")
                 if self.__last_eval_timestamp < source.last_reload_timestamp:
+                    print(f"proxy reloading {source}")
+                    print(self.__value)
                     self.__value = f()
                     self.__last_eval_timestamp = time.time()
-                return getattr(self.__value, name)
+
+            def __getattr__(self, name):
+                self.reload()
+                ret = getattr(self.__value, name)
+                print(f"proxy {name}: {ret}")
+
+                def reloader():
+                    self.reload()
+                    return getattr(self.__value, name)
+                return source.proxy(reloader, type(ret))
         return KebabProxy()
 
     @deprecated_alias(default_value="default")
     def get(
         self,
         config_name=".",
         default=None,
@@ -244,23 +262,23 @@
         Otherwise, it could return None.
 
         Note that the type of the default becomes the expected_type if presents,
         the original expected_type will be ignored in that case.
 
         The parameter `default_value` is deprecated, use `default` instead
         """
-        if update_after_reload and expected_type not in (
-            int, str, float, bool, type(None)
-        ):
+        if update_after_reload:
+            # noinspection PyTypeChecker
             return self.proxy(lambda: self.get(
                 config_name,
                 default,
                 required,
                 expected_type,
-                masked))
+                masked
+            ), expected_type=expected_type)
 
         if default is not None:
             # set expected type based on default value (and ignore the original
             # expected_type
             if expected_type is not None and not isinstance(default, expected_type):
                 raise ValueError(
                     "You specified default of type {}, but expected_type={}".format(
```

### Comparing `pykebab-0.7.4/kebab/utils.py` & `pykebab-0.7.5/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.4/pyproject.toml` & `pykebab-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.7.4/PKG-INFO` & `pykebab-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

