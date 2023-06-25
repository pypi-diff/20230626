# Comparing `tmp/tomfoolery-0.0.0.tar.gz` & `tmp/tomfoolery-0.1.0.tar.gz`

## Comparing `tomfoolery-0.0.0.tar` & `tomfoolery-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/src/tomfoolery/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/src/tomfoolery/_dump.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/src/tomfoolery/_load.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/src/tomfoolery/cli.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/src/tomfoolery/engine.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/src/tomfoolery/utilities.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/README.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tomfoolery-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/_dump.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/_load.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/cli.py
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/engine.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/utilities.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/README.md
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/PKG-INFO
```

### Comparing `tomfoolery-0.0.0/src/tomfoolery/cli.py` & `tomfoolery-0.1.0/src/tomfoolery/cli.py`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.0.0/src/tomfoolery/engine.py` & `tomfoolery-0.1.0/src/tomfoolery/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 from typing import Any
 
 import black
+import isort
 from pathier import Pathier, Pathish
 
 from tomfoolery import utilities
 
 root = Pathier(__file__).parent
 
 
@@ -17,14 +18,18 @@
 
     @property
     def source(self) -> str:
         """Returns the source code this object represents."""
         self.module.body = [self.imports, self.classes]  # type: ignore
         return ast.unparse(self.module)
 
+    def format_str(self, code: str) -> str:
+        """Sort imports and format with `black`."""
+        return black.format_str(isort.api.sort_code_string(code), mode=black.Mode())  # type: ignore
+
     # Seat |===================================== Import Nodes =====================================|
 
     @property
     def dacite_import_node(self) -> ast.Import:
         return ast.Import([ast.alias("dacite")])
 
     @property
@@ -146,11 +151,11 @@
 
         If `write_result` is `True`, the source code will be written to a file of the same name as `path`, but with a `.py` extension."""
         path = Pathier(path)
         name = path.stem
         data = path.loads()
         src = self.generate(name, data)
         src = src.replace("filepath", path.name)
-        src = black.format_str(src, mode=black.Mode())  # type: ignore
+        src = self.format_str(src)
         if write_result:
             path.with_suffix(".py").write_text(src)
         return src
```

### Comparing `tomfoolery-0.0.0/src/tomfoolery/utilities.py` & `tomfoolery-0.1.0/src/tomfoolery/utilities.py`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.0.0/LICENSE.txt` & `tomfoolery-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.0.0/README.md` & `tomfoolery-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.0.0/pyproject.toml` & `tomfoolery-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tomfoolery"
 description = "CLI to generate Python dataclasses that model and load toml files (or other can-representated-as-a-dict files)"
-version = "0.0.0"
+version = "0.1.0"
 requires-python = ">=3.10"
-dependencies = ["pathier", "black", "dacite", "typing_extensions", "pytest"]
+dependencies = ["pathier", "black", "dacite", "typing_extensions", "pytest", "isort"]
 readme = "README.md"
 keywords = ["dataclass", "dataclasses", "toml", "json"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 
 [[project.authors]]
 name = "Matt Manes"
 email = "mattmanes@pm.me"
```

### Comparing `tomfoolery-0.0.0/PKG-INFO` & `tomfoolery-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tomfoolery
-Version: 0.0.0
+Version: 0.1.0
 Summary: CLI to generate Python dataclasses that model and load toml files (or other can-representated-as-a-dict files)
 Project-URL: Homepage, https://github.com/matt-manes/tomfoolery
 Project-URL: Documentation, https://github.com/matt-manes/tomfoolery/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/tomfoolery/tree/main/src/tomfoolery
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: dataclass,dataclasses,json,toml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: black
 Requires-Dist: dacite
+Requires-Dist: isort
 Requires-Dist: pathier
 Requires-Dist: pytest
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # tomfoolery
```

