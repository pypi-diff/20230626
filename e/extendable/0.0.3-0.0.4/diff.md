# Comparing `tmp/extendable-0.0.3.tar.gz` & `tmp/extendable-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extendable-0.0.3.tar", last modified: Tue Nov  1 09:51:16 2022, max compression
+gzip compressed data, was "extendable-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `extendable-0.0.3.tar` & `extendable-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1081 2021-12-20 15:39:04.562356 extendable-0.0.3/LICENSE
--rw-r--r--   0        0        0     3245 2022-06-15 14:05:15.059085 extendable-0.0.3/README.md
--rw-r--r--   0        0        0     1457 2022-06-15 14:16:33.525761 extendable-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      393 2021-12-24 12:52:24.034138 extendable-0.0.3/src/extendable/__init__.py
--rw-r--r--   0        0        0      298 2021-12-22 17:48:19.539244 extendable-0.0.3/src/extendable/context.py
--rw-r--r--   0        0        0     8483 2022-11-01 09:26:41.033458 extendable-0.0.3/src/extendable/main.py
--rw-r--r--   0        0        0        0 2021-12-27 11:01:43.563093 extendable-0.0.3/src/extendable/py.typed
--rw-r--r--   0        0        0     8185 2022-06-15 11:48:30.182431 extendable-0.0.3/src/extendable/registry.py
--rw-r--r--   0        0        0     1059 2021-12-22 18:05:10.232479 extendable-0.0.3/src/extendable/utils.py
--rw-r--r--   0        0        0       22 2022-11-01 09:26:46.045536 extendable-0.0.3/src/extendable/version.py
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2021-12-20 15:39:04.562356 extendable-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3245 2022-06-15 14:05:15.059085 extendable-0.0.4/README.md
+-rw-r--r--   0        0        0     1457 2022-06-15 14:16:33.525761 extendable-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      393 2021-12-24 12:52:24.034138 extendable-0.0.4/src/extendable/__init__.py
+-rw-r--r--   0        0        0      298 2021-12-22 17:48:19.539244 extendable-0.0.4/src/extendable/context.py
+-rw-r--r--   0        0        0     9093 2023-06-26 08:24:33.249690 extendable-0.0.4/src/extendable/main.py
+-rw-r--r--   0        0        0        0 2021-12-27 11:01:43.563093 extendable-0.0.4/src/extendable/py.typed
+-rw-r--r--   0        0        0     8193 2023-06-26 08:24:33.249690 extendable-0.0.4/src/extendable/registry.py
+-rw-r--r--   0        0        0     1059 2021-12-22 18:05:10.232479 extendable-0.0.4/src/extendable/utils.py
+-rw-r--r--   0        0        0       22 2023-06-26 08:25:35.874619 extendable-0.0.4/src/extendable/version.py
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-0.0.4/PKG-INFO
```

### Comparing `extendable-0.0.3/LICENSE` & `extendable-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable-0.0.3/README.md` & `extendable-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `extendable-0.0.3/pyproject.toml` & `extendable-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable-0.0.3/src/extendable/main.py` & `extendable-0.0.4/src/extendable/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,29 @@
 
     def __repr__(self) -> str:
         return (
             f"ExtendableClassDef {self.name} "
             f"{self.namespace['__module__']}.{self.namespace['__qualname__']}"
         )
 
+    def clone(self) -> "ExtendableClassDef":
+        """Clone the class definition, but not the class itself nor the information
+        about the hierarchy.
+
+        This is used to allow to recompute the registry from scratch by
+        starting from the original class definition. This definition is
+        then modified by the build process to define the class
+        hierarchy.
+        """
+        clone = ExtendableClassDef(
+            self.original_name, self.others_bases, self.namespace, self.metaclass
+        )
+        clone.original_cls = self.original_cls
+        return clone
+
 
 _extendable_class_defs_by_module: OrderedDict[
     str, List[ExtendableClassDef]
 ] = collections.OrderedDict()
 
 
 def __register_class_def__(module: str, cls_def: ExtendableClassDef) -> None:
@@ -160,15 +175,15 @@
         """
         return super().__new__(metacls, name, bases, namespace, **kwargs)
 
     @classmethod
     def _wrap_class_methods(metacls, namespace: Dict[str, Any]) -> Dict[str, Any]:
         """Wrap classmethods defined into the namespace to delegate the call to the
         final class."""
-        new_namespace = {}
+        new_namespace: Dict[str, Any] = {}
         for key, value in namespace.items():
             if isinstance(value, classmethod):
                 func = value.__func__
 
                 @no_type_check
                 def new_method(
                     cls, *args, _method_name=None, _initial_func=None, **kwargs
```

### Comparing `extendable-0.0.3/src/extendable/registry.py` & `extendable-0.0.4/src/extendable/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def __iter__(self) -> Iterator[str]:
         return self._extendable_classes.__iter__()
 
     def load_extendable_classes(self, module: str) -> None:
         if module in self._loaded_modules:
             return
         for cls_def in main._extendable_class_defs_by_module.get(module, []):
-            self.load_extendable_class_def(cls_def)
+            self.load_extendable_class_def(cls_def.clone())
         self._loaded_modules.add(module)
 
     def load_extendable_class_def(self, cls_def: main.ExtendableClassDef) -> None:
         parents = cls_def.base_names
         if cls_def.name in self and not parents:
             raise TypeError(
                 f"extendable {cls_def.name} (in class def {cls_def}) already exists."
```

### Comparing `extendable-0.0.3/src/extendable/utils.py` & `extendable-0.0.4/src/extendable/utils.py`

 * *Files identical despite different names*

### Comparing `extendable-0.0.3/PKG-INFO` & `extendable-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lib to define class extendable at runtime.
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

