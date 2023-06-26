# Comparing `tmp/pyrdfj2-0.0.2.tar.gz` & `tmp/pyrdfj2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdfj2-0.0.2.tar", max compression
+gzip compressed data, was "pyrdfj2-0.0.3.tar", max compression
```

## Comparing `pyrdfj2-0.0.2.tar` & `pyrdfj2-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/LICENSE
--rw-r--r--   0        0        0      870 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/README.rst
--rw-r--r--   0        0        0     1955 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      233 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyrdfj2/__init__.py
--rw-r--r--   0        0        0       79 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyrdfj2/__version__.py
--rw-r--r--   0        0        0      313 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyrdfj2/exceptions.py
--rw-r--r--   0        0        0     5633 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyrdfj2/j2_functions.py
--rw-r--r--   0        0        0      812 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyrdfj2/pyrdfj2.py
--rw-r--r--   0        0        0     2483 2023-06-14 07:10:12.750340 pyrdfj2-0.0.2/pyrdfj2/rdf_syntax_builder.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 pyrdfj2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-26 06:56:52.297906 pyrdfj2-0.0.3/LICENSE
+-rw-r--r--   0        0        0      870 2023-06-26 06:56:52.297906 pyrdfj2-0.0.3/README.rst
+-rw-r--r--   0        0        0     1955 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      229 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyrdfj2/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyrdfj2/__version__.py
+-rw-r--r--   0        0        0      313 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyrdfj2/exceptions.py
+-rw-r--r--   0        0        0     5734 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyrdfj2/j2_functions.py
+-rw-r--r--   0        0        0      812 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyrdfj2/pyrdfj2.py
+-rw-r--r--   0        0        0     2538 2023-06-26 06:56:52.301906 pyrdfj2-0.0.3/pyrdfj2/syntax_builder.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 pyrdfj2-0.0.3/PKG-INFO
```

### Comparing `pyrdfj2-0.0.2/LICENSE` & `pyrdfj2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdfj2-0.0.2/README.rst` & `pyrdfj2-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyrdfj2-0.0.2/pyproject.toml` & `pyrdfj2-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrdfj2"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python wrapper on jinja SPARQL templating"
 authors = [ "Marc Portier <marc.portier@gmail.com>", 
             "João Santos <jotaflame@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "pyrdfj2"}]
 license = "MIT"
```

### Comparing `pyrdfj2-0.0.2/pyrdfj2/j2_functions.py` & `pyrdfj2-0.0.3/pyrdfj2/j2_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
     @staticmethod
     def all():
         return {
             "uritexpand": uritexpand,
             "regexreplace": regexreplace,
             "map": map_build,
+            # TODO: Check for duplication in filters and the meaning.
+            "xsd": xsd_format,
         }
 
 
 class Filters:
     @staticmethod
     def all():
         return {
```

### Comparing `pyrdfj2-0.0.2/pyrdfj2/pyrdfj2.py` & `pyrdfj2-0.0.3/pyrdfj2/pyrdfj2.py`

 * *Files identical despite different names*

### Comparing `pyrdfj2-0.0.2/pyrdfj2/rdf_syntax_builder.py` & `pyrdfj2-0.0.3/pyrdfj2/syntax_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,20 @@
     """
 
     def __init__(
         self,
         templates_folder: str = "",
         extra_filters={},
         extra_functions={},
+        jinja_env_variables={},
     ):
         if not templates_folder:
             raise NoTemplateFolder
         self._templates_env = Environment(
-            loader=FileSystemLoader(templates_folder)
+            loader=FileSystemLoader(templates_folder), **jinja_env_variables
         )
 
         filters: dict = Filters.all()
         functions: dict = Functions.all()
         if extra_filters:
             filters.update(extra_filters)
         if extra_functions:
```

### Comparing `pyrdfj2-0.0.2/PKG-INFO` & `pyrdfj2-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfj2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper on jinja SPARQL templating
 Home-page: https://github.com/vliz-be-opsci/pyrdfj2
 License: MIT
 Author: Marc Portier
 Author-email: marc.portier@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

