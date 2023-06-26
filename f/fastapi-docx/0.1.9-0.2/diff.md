# Comparing `tmp/fastapi_docx-0.1.9.tar.gz` & `tmp/fastapi_docx-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_docx-0.1.9.tar", max compression
+gzip compressed data, was "fastapi_docx-0.2.tar", max compression
```

## Comparing `fastapi_docx-0.1.9.tar` & `fastapi_docx-0.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-01-02 14:16:32.954764 fastapi_docx-0.1.9/LICENSE
--rw-r--r--   0        0        0     2371 2023-01-28 19:02:18.558491 fastapi_docx-0.1.9/README.md
--rw-r--r--   0        0        0       78 2023-01-02 14:34:42.780644 fastapi_docx-0.1.9/fastapi_docx/__init__.py
--rw-r--r--   0        0        0    14546 2023-04-02 21:49:21.245448 fastapi_docx-0.1.9/fastapi_docx/exception_finder.py
--rw-r--r--   0        0        0     3408 2023-01-02 19:37:11.768694 fastapi_docx-0.1.9/fastapi_docx/openapi.py
--rw-r--r--   0        0        0        0 2023-03-18 18:50:29.161351 fastapi_docx-0.1.9/fastapi_docx/py.typed
--rw-r--r--   0        0        0     2518 2023-01-02 19:37:11.768947 fastapi_docx-0.1.9/fastapi_docx/response_generator.py
--rw-r--r--   0        0        0     1996 2023-04-02 21:51:48.466548 fastapi_docx-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 fastapi_docx-0.1.9/setup.py
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fastapi_docx-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-26 11:11:07.109320 fastapi_docx-0.2/LICENSE
+-rw-r--r--   0        0        0     2371 2023-06-26 12:30:17.579687 fastapi_docx-0.2/README.md
+-rw-r--r--   0        0        0       78 2023-06-26 11:11:07.115029 fastapi_docx-0.2/fastapi_docx/__init__.py
+-rw-r--r--   0        0        0    16510 2023-06-26 12:55:00.875540 fastapi_docx-0.2/fastapi_docx/exception_finder.py
+-rw-r--r--   0        0        0     3408 2023-06-26 11:11:07.115284 fastapi_docx-0.2/fastapi_docx/openapi.py
+-rw-r--r--   0        0        0        0 2023-06-26 11:11:07.115316 fastapi_docx-0.2/fastapi_docx/py.typed
+-rw-r--r--   0        0        0     2518 2023-06-26 11:11:07.115414 fastapi_docx-0.2/fastapi_docx/response_generator.py
+-rw-r--r--   0        0        0     1994 2023-06-26 12:13:17.043032 fastapi_docx-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 fastapi_docx-0.2/PKG-INFO
```

### Comparing `fastapi_docx-0.1.9/LICENSE` & `fastapi_docx-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_docx-0.1.9/README.md` & `fastapi_docx-0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_docx-0.1.9/fastapi_docx/exception_finder.py` & `fastapi_docx-0.2/fastapi_docx/exception_finder.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,18 +76,68 @@
     exc_class: type[Exception], exc_args: list[Any] | None = None
 ) -> Exception | None:
     importlib.import_module(exc_class.__module__)
     value = exc_class(*exc_args) if exc_args else exc_class()
     return value if isinstance(value, Exception) else None
 
 
+def replace_binops(node: ast.AST) -> None:
+    """Replace binary addition operations with their string representation."""
+    for name, field in ast.iter_fields(node):
+        if isinstance(field, list):
+            for i, item in enumerate(field):
+                if isinstance(item, ast.BinOp) and isinstance(item.op, ast.Add):
+                    field[i] = ast.Constant(
+                        value=f"<{ast.unparse(item.left)}> + <{ast.unparse(item.right)}>"
+                    )
+                else:
+                    replace_binops(item)
+        elif isinstance(field, ast.AST):
+            if isinstance(field, ast.BinOp) and isinstance(field.op, ast.Add):
+                setattr(
+                    node,
+                    name,
+                    ast.Constant(
+                        value=f"<{ast.unparse(field.left)}> + <{ast.unparse(field.right)}>"
+                    ),
+                )
+            else:
+                replace_binops(field)
+
+
+def replace_formatted_values(node: ast.AST) -> None:
+    """Replace formatted values with their string representation."""
+    for name, field in ast.iter_fields(node):
+        if isinstance(field, list):
+            for i, item in enumerate(field):
+                if isinstance(item, ast.FormattedValue):
+                    field[i] = ast.Constant(
+                        value=f"<{ast.unparse(item.value).upper()}>"
+                    )
+                else:
+                    replace_formatted_values(item)
+                    replace_binops(item)
+        elif isinstance(field, ast.AST):
+            if isinstance(field, ast.FormattedValue):
+                setattr(
+                    node,
+                    name,
+                    ast.Constant(value=f"<{ast.unparse(field.value).upper()}>"),
+                )
+            else:
+                replace_formatted_values(field)
+                replace_binops(field)
+    return None
+
+
 def eval_ast_exc_instance(
     exc_class: type[Exception], ast_exec_inst: ast.expr
 ) -> Exception | None:
     importlib.import_module(exc_class.__module__)
+    replace_formatted_values(ast_exec_inst)
     value = eval(ast.unparse(ast_exec_inst))
     return value if isinstance(value, Exception) else None
 
 
 class RouteExcFinder:
     def __init__(
         self,
@@ -298,15 +348,14 @@
 
     def create_exc_inst_from_raise_stmt(
         self,
         raise_stmt: ast.Raise,
         module: ModuleType | type,
     ) -> Exception | None:
         if raise_stmt.exc and hasattr(raise_stmt.exc, "func"):
-
             if hasattr(raise_stmt.exc.func, "attr"):
                 try:
                     outer_exc_class = getattr(
                         module,
                         raise_stmt.exc.func.value.id,
                     )
                     http_exc = getattr(outer_exc_class, raise_stmt.exc.func.attr)
```

### Comparing `fastapi_docx-0.1.9/fastapi_docx/openapi.py` & `fastapi_docx-0.2/fastapi_docx/openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_docx-0.1.9/fastapi_docx/response_generator.py` & `fastapi_docx-0.2/fastapi_docx/response_generator.py`

 * *Files identical despite different names*

### Comparing `fastapi_docx-0.1.9/pyproject.toml` & `fastapi_docx-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-docx"
-version = "0.1.9"
+version = "0.2"
 description = "Extend a FastAPI OpenAPI spec to include all possible HTTPException or custom Exception response schemas."
 authors = ["Saran Connolly <saran@example.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/Saran33/fastapi-docx"
 
 classifiers = [
```

### Comparing `fastapi_docx-0.1.9/setup.py` & `fastapi_docx-0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,65 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-docx
+Version: 0.2
+Summary: Extend a FastAPI OpenAPI spec to include all possible HTTPException or custom Exception response schemas.
+Home-page: https://github.com/Saran33/fastapi-docx
+License: MIT
+Author: Saran Connolly
+Author-email: saran@example.com
+Requires-Python: >=3.10,<4.0.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: fastapi (>=0.88.0)
+Project-URL: Repository, https://github.com/Saran33/fastapi-docx
+Description-Content-Type: text/markdown
+
+# fastapi-docx
+
+<p align="center">
+  <a href="https://github.com/Saran33/fastapi-docx"><img src="https://saran33.github.io/fastapi-docx/img/fastapi-docx-logo-teal.png" alt="FastAPI"></a>
+</p>
+<p align="center">
+    <em>Add HTTPException responses to a FastAPI OpenAPI spec</em>
+</p>
+<p align="center">
+<a href="https://github.com/saran33/fastapi-docx/actions?query=workflow%3ACI+event%3Apush+branch%3Amain" target="_blank">
+    <img src="https://github.com/saran33/fastapi-docx/workflows/CI/badge.svg?event=push&branch=main" alt="CI">
+</a>
+<a href="https://saran33.github.io/fastapi-docx/coverage/coverage.html" target="_blank">
+    <img src="https://saran33.github.io/fastapi-docx/coverage/coverage-badge.svg" alt="Coverage">
+</a>
+<a href="https://pypi.org/project/fastapi-docx" target="_blank">
+    <img src="https://img.shields.io/pypi/v/fastapi-docx?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/fastapi-docx" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/fastapi-docx" alt="Supported Python versions">
+</a>
+</p>
+
+---
+
+**Documentation**: <a href="https://saran33.github.io/fastapi-docx" target="_blank">https://saran33.github.io/fastapi-docx</a>
+
+**Source Code**: <a href="https://github.com/Saran33/fastapi-docx" target="_blank">https://github.com/Saran33/fastapi-docx</a>
+
+---
+
+FastAPI-docx extends the FastAPI OpenAPI spec to include all possible `HTTPException` or custom Exception response schemas that may be raised within path operations.
+
+The key features are:
+
+* **Document Exception Responses**: Automatically find all possible respones within path operations, whether they originate from a `HTTPException` raised by the endpoint function directly, in a nested function, class method, or callable class instance, or by the fastAPI dependency-injection system.
+* **Include Custom Exceptions**: Optionally find and document any custom Exception types if using custom Exception handlers in your FastAPI application.
+* **Generate Exception schemas**: A default `HTTPExceptionSchema` will be added to the OpenAPI specification. The default can be modified to use any other [Pydantic](*https://github.com/pydantic/pydantic) model. An additional schema for app-specific custom Exceptions can also be included.
 
-packages = \
-['fastapi_docx']
+##### License
+This project is licensed under the terms of the MIT license.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fastapi>=0.88.0']
-
-setup_kwargs = {
-    'name': 'fastapi-docx',
-    'version': '0.1.9',
-    'description': 'Extend a FastAPI OpenAPI spec to include all possible HTTPException or custom Exception response schemas.',
-    'long_description': '# fastapi-docx\n\n<p align="center">\n  <a href="https://github.com/Saran33/fastapi-docx"><img src="https://saran33.github.io/fastapi-docx/img/fastapi-docx-logo-teal.png" alt="FastAPI"></a>\n</p>\n<p align="center">\n    <em>Add HTTPException responses to a FastAPI OpenAPI spec</em>\n</p>\n<p align="center">\n<a href="https://github.com/saran33/fastapi-docx/actions?query=workflow%3ACI+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/saran33/fastapi-docx/workflows/CI/badge.svg?event=push&branch=main" alt="CI">\n</a>\n<a href="https://saran33.github.io/fastapi-docx/coverage/coverage.html" target="_blank">\n    <img src="https://saran33.github.io/fastapi-docx/coverage/coverage-badge.svg" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/fastapi-docx" target="_blank">\n    <img src="https://img.shields.io/pypi/v/fastapi-docx?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/fastapi-docx" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/fastapi-docx" alt="Supported Python versions">\n</a>\n</p>\n\n---\n\n**Documentation**: <a href="https://saran33.github.io/fastapi-docx" target="_blank">https://saran33.github.io/fastapi-docx</a>\n\n**Source Code**: <a href="https://github.com/Saran33/fastapi-docx" target="_blank">https://github.com/Saran33/fastapi-docx</a>\n\n---\n\nFastAPI-docx extends the FastAPI OpenAPI spec to include all possible `HTTPException` or custom Exception response schemas that may be raised within path operations.\n\nThe key features are:\n\n* **Document Exception Responses**: Automatically find all possible respones within path operations, whether they originate from a `HTTPException` raised by the endpoint function directly, in a nested function, class method, or callable class instance, or by the fastAPI dependency-injection system.\n* **Include Custom Exceptions**: Optionally find and document any custom Exception types if using custom Exception handlers in your FastAPI application.\n* **Generate Exception schemas**: A default `HTTPExceptionSchema` will be added to the OpenAPI specification. The default can be modified to use any other [Pydantic](*https://github.com/pydantic/pydantic) model. An additional schema for app-specific custom Exceptions can also be included.\n\n##### License\nThis project is licensed under the terms of the MIT license.\n',
-    'author': 'Saran Connolly',
-    'author_email': 'saran@example.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Saran33/fastapi-docx',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['fastapi_docx'] package_data = \ {'': ['*']} install_requires = \
-['fastapi>=0.88.0'] setup_kwargs = { 'name': 'fastapi-docx', 'version':
-'0.1.9', 'description': 'Extend a FastAPI OpenAPI spec to include all possible
-HTTPException or custom Exception response schemas.', 'long_description': '#
-fastapi-docx\n\n
-                                \n [FastAPI]\n
-\n
-          \n Add HTTPException responses to a FastAPI OpenAPI spec\n
-\n
-  \n\n_[CI]\n\n\n_[Coverage]\n\n\n_[Package_version]\n\n\n_[Supported_Python
-                                 versions]\n\n
-\n\n---\n\n**Documentation**: https://saran33.github.io/fastapi-
-docx\n\n**Source Code**: https://github.com/Saran33/fastapi-docx\n\n---
-\n\nFastAPI-docx extends the FastAPI OpenAPI spec to include all possible
-`HTTPException` or custom Exception response schemas that may be raised within
-path operations.\n\nThe key features are:\n\n* **Document Exception
-Responses**: Automatically find all possible respones within path operations,
-whether they originate from a `HTTPException` raised by the endpoint function
-directly, in a nested function, class method, or callable class instance, or by
-the fastAPI dependency-injection system.\n* **Include Custom Exceptions**:
-Optionally find and document any custom Exception types if using custom
-Exception handlers in your FastAPI application.\n* **Generate Exception
-schemas**: A default `HTTPExceptionSchema` will be added to the OpenAPI
-specification. The default can be modified to use any other [Pydantic](*https:/
-/github.com/pydantic/pydantic) model. An additional schema for app-specific
-custom Exceptions can also be included.\n\n##### License\nThis project is
-licensed under the terms of the MIT license.\n', 'author': 'Saran Connolly',
-'author_email': 'saran@example.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/Saran33/fastapi-docx', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.10,<4.0.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: fastapi-docx Version: 0.2 Summary: Extend a FastAPI
+OpenAPI spec to include all possible HTTPException or custom Exception response
+schemas. Home-page: https://github.com/Saran33/fastapi-docx License: MIT
+Author: Saran Connolly Author-email: saran@example.com Requires-Python:
+>=3.10,<4.0.0 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: fastapi (>=0.88.0) Project-URL: Repository, https://github.com/
+Saran33/fastapi-docx Description-Content-Type: text/markdown # fastapi-docx
+                                   [FastAPI]
+             Add HTTPException responses to a FastAPI OpenAPI spec
+         [CI] [Coverage] [Package_version] [Supported_Python_versions]
+--- **Documentation**: https://saran33.github.io/fastapi-docx **Source Code**:
+https://github.com/Saran33/fastapi-docx --- FastAPI-docx extends the FastAPI
+OpenAPI spec to include all possible `HTTPException` or custom Exception
+response schemas that may be raised within path operations. The key features
+are: * **Document Exception Responses**: Automatically find all possible
+respones within path operations, whether they originate from a `HTTPException`
+raised by the endpoint function directly, in a nested function, class method,
+or callable class instance, or by the fastAPI dependency-injection system. *
+**Include Custom Exceptions**: Optionally find and document any custom
+Exception types if using custom Exception handlers in your FastAPI application.
+* **Generate Exception schemas**: A default `HTTPExceptionSchema` will be added
+to the OpenAPI specification. The default can be modified to use any other
+[Pydantic](*https://github.com/pydantic/pydantic) model. An additional schema
+for app-specific custom Exceptions can also be included. ##### License This
+project is licensed under the terms of the MIT license.
```

