# Comparing `tmp/arxlang-0.1.0.tar.gz` & `tmp/arxlang-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxlang-0.1.0.tar", max compression
+gzip compressed data, was "arxlang-0.1.1.tar", max compression
```

## Comparing `arxlang-0.1.0.tar` & `arxlang-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      585 2023-06-11 16:55:11.995688 arxlang-0.1.0/LICENSE
--rw-r--r--   0        0        0     1834 2023-06-20 02:50:54.684323 arxlang-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      475 2023-06-16 04:30:48.023088 arxlang-0.1.0/src/arx/__init__.py
--rw-r--r--   0        0        0      367 2023-06-11 17:20:48.308781 arxlang-0.1.0/src/arx/__main__.py
--rw-r--r--   0        0        0     5888 2023-06-20 00:31:40.102546 arxlang-0.1.0/src/arx/ast.py
--rw-r--r--   0        0        0     2459 2023-06-19 23:00:47.633432 arxlang-0.1.0/src/arx/cli.py
--rw-r--r--   0        0        0       42 2023-06-16 03:02:20.927165 arxlang-0.1.0/src/arx/codegen/__init__.py
--rw-r--r--   0        0        0     7334 2023-06-20 00:31:49.194590 arxlang-0.1.0/src/arx/codegen/ast_output.py
--rw-r--r--   0        0        0     5448 2023-06-20 00:50:12.567078 arxlang-0.1.0/src/arx/codegen/base.py
--rw-r--r--   0        0        0    20471 2023-06-20 00:42:49.849487 arxlang-0.1.0/src/arx/codegen/file_object.py
--rw-r--r--   0        0        0     3619 2023-06-19 23:05:38.215790 arxlang-0.1.0/src/arx/io.py
--rw-r--r--   0        0        0     6590 2023-06-18 21:09:51.578093 arxlang-0.1.0/src/arx/lexer.py
--rw-r--r--   0        0        0      406 2023-06-16 03:00:52.516111 arxlang-0.1.0/src/arx/logs.py
--rw-r--r--   0        0        0     1634 2023-06-20 00:07:40.339414 arxlang-0.1.0/src/arx/main.py
--rw-r--r--   0        0        0    17655 2023-06-20 00:34:55.643544 arxlang-0.1.0/src/arx/parser.py
--rw-r--r--   0        0        0       32 2023-06-16 02:27:00.025413 arxlang-0.1.0/src/arx/semantic.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 arxlang-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-06-26 03:49:55.936740 arxlang-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1893 2023-06-26 03:52:24.857469 arxlang-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      475 2023-06-26 03:52:24.853469 arxlang-0.1.1/src/arx/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/__main__.py
+-rw-r--r--   0        0        0     5888 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/ast.py
+-rw-r--r--   0        0        0     2459 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/cli.py
+-rw-r--r--   0        0        0       42 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/codegen/__init__.py
+-rw-r--r--   0        0        0     7334 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/codegen/ast_output.py
+-rw-r--r--   0        0        0     5448 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/codegen/base.py
+-rw-r--r--   0        0        0    20471 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/codegen/file_object.py
+-rw-r--r--   0        0        0     3619 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/io.py
+-rw-r--r--   0        0        0     6590 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/lexer.py
+-rw-r--r--   0        0        0      406 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/logs.py
+-rw-r--r--   0        0        0     1634 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/main.py
+-rw-r--r--   0        0        0    17655 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/parser.py
+-rw-r--r--   0        0        0       32 2023-06-26 03:49:55.940740 arxlang-0.1.1/src/arx/semantic.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 arxlang-0.1.1/PKG-INFO
```

### Comparing `arxlang-0.1.0/LICENSE` & `arxlang-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/pyproject.toml` & `arxlang-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arxlang"
-version = "0.1.0"  # semantic-release
+version = "0.1.1"  # semantic-release
 description = "Arx is a compiler built with llvm"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "Apache Software License 2.0"
 include = [
   "src/arx",
 ]
 exclude = [
@@ -39,14 +39,15 @@
 mkdocs-exclude = ">=1.0.2,<2"
 mkdocs-jupyter = ">=0.20.0,<1"
 mkdocs-literate-nav = ">=0.4.1,<1"
 mkdocs-macros-plugin = ">=0.6.3,<1"
 mkdocs-material = ">=8.2.1,<9"
 mkdocstrings = ">=0.17.0,<0.18.0"
 makim = "1.8.1"
+pytkdocs = {extras = ["numpy-style"], version = "^0.16.1"}
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.mypy]
```

### Comparing `arxlang-0.1.0/src/arx/ast.py` & `arxlang-0.1.1/src/arx/ast.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/cli.py` & `arxlang-0.1.1/src/arx/cli.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/codegen/ast_output.py` & `arxlang-0.1.1/src/arx/codegen/ast_output.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/codegen/base.py` & `arxlang-0.1.1/src/arx/codegen/base.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/codegen/file_object.py` & `arxlang-0.1.1/src/arx/codegen/file_object.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/io.py` & `arxlang-0.1.1/src/arx/io.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/lexer.py` & `arxlang-0.1.1/src/arx/lexer.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/main.py` & `arxlang-0.1.1/src/arx/main.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/src/arx/parser.py` & `arxlang-0.1.1/src/arx/parser.py`

 * *Files identical despite different names*

### Comparing `arxlang-0.1.0/PKG-INFO` & `arxlang-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxlang
-Version: 0.1.0
+Version: 0.1.1
 Summary: Arx is a compiler built with llvm
 License: Apache Software License 2.0
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

