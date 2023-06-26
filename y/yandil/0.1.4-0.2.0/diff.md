# Comparing `tmp/yandil-0.1.4.tar.gz` & `tmp/yandil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.1.4.tar", max compression
+gzip compressed data, was "yandil-0.2.0.tar", max compression
```

## Comparing `yandil-0.1.4.tar` & `yandil-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11358 2023-06-24 09:57:46.611151 yandil-0.1.4/README.md
--rw-r--r--   0        0        0      817 2023-06-24 09:58:40.774123 yandil-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    10627 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/dependency.py
--rw-r--r--   0        0        0     1020 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     2364 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-24 09:57:46.611151 yandil-0.1.4/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11505 2023-06-26 15:52:42.050674 yandil-0.2.0/README.md
+-rw-r--r--   0        0        0      817 2023-06-26 15:53:40.874952 yandil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    10627 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1020 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     3548 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-26 15:52:42.050674 yandil-0.2.0/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    11836 1970-01-01 00:00:00.000000 yandil-0.2.0/PKG-INFO
```

### Comparing `yandil-0.1.4/README.md` & `yandil-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 from yandil.container import default_container
 ```
 
 In order to tune the dependency injection discovery process the loader has the following options:
 - **excluded_modules**: Set of module or package names to be excluded from the dependency injection discovery process. For example for excluding the folder which contains the models in a web application.
 - **should_exclude_classes_without_public_methods**: If set to True, classes which not define any public method will be excluded from the dependency injection discovery process. For example for excluding DTO classes.
 - **should_exclude_dataclasses**: If set to True, dataclasses will be excluded from the dependency injection discovery process.
+- **mandatory_modules**: Set of module paths which classes contained should be loaded as dependencies without checking if they meet any condition.
 
 ### Declarative way
 In this way you will need to decorate the classes which you want to be loaded as dependencies.
 
 Giving the following python project structure:
 ```
 ├── app
```

### Comparing `yandil-0.1.4/pyproject.toml` & `yandil-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.1.4"
+version = "0.2.0"
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
-version = "0.1.4"
+version = "0.2.0"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.1.4/src/yandil/configuration/configuration_container.py` & `yandil-0.2.0/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/container.py` & `yandil-0.2.0/src/yandil/container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/declarative/decorators.py` & `yandil-0.2.0/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/dependency.py` & `yandil-0.2.0/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/dependency_filler.py` & `yandil-0.2.0/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/discovery/class_discovery.py` & `yandil-0.2.0/src/yandil/discovery/class_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/discovery/module_discovery.py` & `yandil-0.2.0/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.2.0/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/src/yandil/typing_tools.py` & `yandil-0.2.0/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.4/PKG-INFO` & `yandil-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.1.4
+Version: 0.2.0
 Summary: Yet ANother Dependency Injection Library
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -82,14 +82,15 @@
 from yandil.container import default_container
 ```
 
 In order to tune the dependency injection discovery process the loader has the following options:
 - **excluded_modules**: Set of module or package names to be excluded from the dependency injection discovery process. For example for excluding the folder which contains the models in a web application.
 - **should_exclude_classes_without_public_methods**: If set to True, classes which not define any public method will be excluded from the dependency injection discovery process. For example for excluding DTO classes.
 - **should_exclude_dataclasses**: If set to True, dataclasses will be excluded from the dependency injection discovery process.
+- **mandatory_modules**: Set of module paths which classes contained should be loaded as dependencies without checking if they meet any condition.
 
 ### Declarative way
 In this way you will need to decorate the classes which you want to be loaded as dependencies.
 
 Giving the following python project structure:
 ```
 ├── app
```

