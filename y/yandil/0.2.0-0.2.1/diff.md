# Comparing `tmp/yandil-0.2.0.tar.gz` & `tmp/yandil-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.2.0.tar", max compression
+gzip compressed data, was "yandil-0.2.1.tar", max compression
```

## Comparing `yandil-0.2.0.tar` & `yandil-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11505 2023-06-26 15:52:42.050674 yandil-0.2.0/README.md
--rw-r--r--   0        0        0      817 2023-06-26 15:53:40.874952 yandil-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    10627 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/dependency.py
--rw-r--r--   0        0        0     1020 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     3548 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11836 1970-01-01 00:00:00.000000 yandil-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11594 2023-06-26 20:49:21.618091 yandil-0.2.1/README.md
+-rw-r--r--   0        0        0      817 2023-06-26 20:50:27.278769 yandil-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    10681 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1020 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     3548 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-26 20:49:21.618091 yandil-0.2.1/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    11925 1970-01-01 00:00:00.000000 yandil-0.2.1/PKG-INFO
```

### Comparing `yandil-0.2.0/README.md` & `yandil-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # YANDIL
 [![YANDIL CI](https://github.com/DeejayRevok/yandil/actions/workflows/pythonapp.yml/badge.svg?branch=main)](https://github.com/DeejayRevok/yandil/actions/workflows/pythonapp.yml)
+[![PyPI version](https://badge.fury.io/py/yandil.svg)](https://pypi.org/project/yandil/)
 
 ## What is YANDIL?
 YANDIL(**Yet ANother Dependency Injection Library**) is a python dependency injection library with two main aims:
 - **Decouple the application source code totally from the dependency injection schema**.
 - **Avoid the need of dependency injection definitions**.
 
 ## How does it work?
```

### Comparing `yandil-0.2.0/pyproject.toml` & `yandil-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.2.0"
+version = "0.2.1"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 
@@ -30,15 +30,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0"
+version = "0.2.1"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.2.0/src/yandil/configuration/configuration_container.py` & `yandil-0.2.1/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/container.py` & `yandil-0.2.1/src/yandil/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         self.__bases_map: Dict[Type | GenericAlias, List[Type]] = defaultdict(list)
         self.__configuration_container = configuration_container
 
     def add(self, cls: Type, is_primary: Optional[bool] = None) -> None:
         if self.__is_abstract_class(cls):
             raise AbstractClassNotAllowedError(cls)
 
+        if cls in self.__dependency_map:
+            return
+
         dependency = Dependency(cls, is_primary=is_primary)
 
         self.__update_bases_map(cls, is_primary)
         self.__dependency_map[cls] = dependency
 
     def __setitem__(self, cls: Type[DT], value: DT) -> None:
         if self.__is_abstract_class(cls):
@@ -183,15 +186,15 @@
         optional_inner_type = next(arg for arg in get_args(cls))
         try:
             return self[optional_inner_type]
         except DependencyNotFoundError:
             return None
 
     def __set_arguments(self, dependency: Dependency) -> None:
-        if len(dependency.arguments) > 0:
+        if dependency.is_resolved:
             return
 
         for argument_name, argument_type in get_type_hints(dependency.cls.__init__).items():
             if self.__should_skip_argument(dependency.cls, argument_name):
                 continue
 
             if self.__is_configuration_argument(argument_type):
```

### Comparing `yandil-0.2.0/src/yandil/declarative/decorators.py` & `yandil-0.2.1/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/dependency.py` & `yandil-0.2.1/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/dependency_filler.py` & `yandil-0.2.1/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/discovery/class_discovery.py` & `yandil-0.2.1/src/yandil/discovery/class_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/discovery/module_discovery.py` & `yandil-0.2.1/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.2.1/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.2.1/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/src/yandil/typing_tools.py` & `yandil-0.2.1/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.2.0/PKG-INFO` & `yandil-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.2.0
+Version: 0.2.1
 Summary: Yet ANother Dependency Injection Library
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # YANDIL
 [![YANDIL CI](https://github.com/DeejayRevok/yandil/actions/workflows/pythonapp.yml/badge.svg?branch=main)](https://github.com/DeejayRevok/yandil/actions/workflows/pythonapp.yml)
+[![PyPI version](https://badge.fury.io/py/yandil.svg)](https://pypi.org/project/yandil/)
 
 ## What is YANDIL?
 YANDIL(**Yet ANother Dependency Injection Library**) is a python dependency injection library with two main aims:
 - **Decouple the application source code totally from the dependency injection schema**.
 - **Avoid the need of dependency injection definitions**.
 
 ## How does it work?
```

