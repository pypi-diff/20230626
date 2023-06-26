# Comparing `tmp/clearconf-0.3.1.tar.gz` & `tmp/clearconf-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.1.tar", max compression
+gzip compressed data, was "clearconf-0.3.2.tar", max compression
```

## Comparing `clearconf-0.3.1.tar` & `clearconf-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-06-22 21:13:09.616037 clearconf-0.3.1/README.md
--rw-r--r--   0        0        0       37 2023-06-22 21:13:09.616037 clearconf-0.3.1/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     5834 2023-06-22 22:22:44.826005 clearconf-0.3.1/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      723 2023-06-22 22:26:28.545992 clearconf-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-06-22 21:13:09.616037 clearconf-0.3.2/README.md
+-rw-r--r--   0        0        0       37 2023-06-22 21:13:09.616037 clearconf-0.3.2/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     6347 2023-06-26 12:08:00.831325 clearconf-0.3.2/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      723 2023-06-26 12:08:40.671325 clearconf-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.2/PKG-INFO
```

### Comparing `clearconf-0.3.1/README.md` & `clearconf-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/clearconf/assets/example_conf.py` & `clearconf-0.3.2/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/clearconf/assets/init.py` & `clearconf-0.3.2/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/clearconf/base_config.py` & `clearconf-0.3.2/clearconf/base_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,27 @@
 class BaseConfig(metaclass=Watcher):
 
     @classmethod
     def to_json(cls):
         return json.dumps(cls.to_dict())
 
     @classmethod
-    def to_dict(cls):
+    def to_dict(cls, add_parent=False):
         target = cls
 
-        res = {}
+        # This add target as the top key of the dictionary
+        #  if add_parent is True
+        res = output = {}
+        if add_parent:
+            key = target.__name__
+            if len(target.mro()) >= 4:
+                key =  target.mro()[2].__name__
+            if len(target.mro()) >= 5:
+                key = f'{key}({target.mro()[3].__name__})'
+            output = {key: res}
 
         target_attr = set(dir(target))
         # This removes variables from superclasses
         for i in range(3, len(target.__mro__) - 1):
             # The if allows inheritance between configs but I guess there are better solutions
             if 'configs' not in target.__mro__[i].__module__:
                 target_attr = target_attr - set(dir(target.__mro__[i]))
@@ -45,29 +54,31 @@
                         if attr.__name__ == '<lambda>':
                             funcString = str(inspect.getsourcelines(attr)[0])
                             res[k] = funcString.strip("['\\n']").split(" = ")[1]
                         else:
                             res[k] = f'function : {attr.__name__}'
                     elif attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
                         if len(attr.mro()) >= 5: # when a config class is subclassed to use it directly
-                            k = attr.mro()[3].__name__ 
+                            k = f'{k}({attr.mro()[3].__name__})'
                         res[k] = attr.to_dict()
                     else:
                         # End up here if attr is not a class defined inside module.
-                        # e.g. built-in types, functions, etc.
-                        if type(attr).__name__ == 'type':
+                        if type(attr).__name__ == 'type':  # it is a class
                             name = attr.__name__
-                        else:
+                        else: # it is an object
                             name = type(attr).__name__
+                            if attr.__str__ is not object.__str__:
+                                name = attr.__str__()   
                         res[k] = f'{attr.__module__}.{name}'
                 # If it's not a class save it. This is done for basic types.
                 # Could cause problems with complex objects
                 else:
                     res[k] = attr
-        return res
+
+        return output
 
     @classmethod
     def _subclass(cls):
 
         target = cls
 
         res = {}
```

### Comparing `clearconf-0.3.1/clearconf/cli/defaults.py` & `clearconf-0.3.2/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/clearconf/cli/main.py` & `clearconf-0.3.2/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/clearconf/utils/conf.py` & `clearconf-0.3.2/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/clearconf/utils/file.py` & `clearconf-0.3.2/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.1/pyproject.toml` & `clearconf-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3.1"
+version = "0.3.2"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
 authors = ["andrearosasco <andrea.rosasco@iit.it>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
```

### Comparing `clearconf-0.3.1/PKG-INFO` & `clearconf-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3.1
+Version: 0.3.2
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
 Author: andrearosasco
 Author-email: andrea.rosasco@iit.it
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

