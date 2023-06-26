# Comparing `tmp/decorator_parser-1.0.3.tar.gz` & `tmp/decorator_parser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_parser-1.0.3.tar", last modified: Sun Jun 25 15:51:15 2023, max compression
+gzip compressed data, was "decorator_parser-1.0.4.tar", last modified: Mon Jun 26 10:31:49 2023, max compression
```

## Comparing `decorator_parser-1.0.3.tar` & `decorator_parser-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:51:15.458257 decorator_parser-1.0.3/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      519 2023-06-25 14:29:47.000000 decorator_parser-1.0.3/LICENSE
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4339 2023-06-25 15:51:15.458257 decorator_parser-1.0.3/PKG-INFO
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3829 2023-06-25 15:50:04.000000 decorator_parser-1.0.3/README.md
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      587 2023-06-25 15:51:03.000000 decorator_parser-1.0.3/pyproject.toml
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       38 2023-06-25 15:51:15.458257 decorator_parser-1.0.3/setup.cfg
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:51:15.448257 decorator_parser-1.0.3/src/
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:51:15.458257 decorator_parser-1.0.3/src/decorator_parser/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:21:25.000000 decorator_parser-1.0.3/src/decorator_parser/__init__.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     1093 2023-06-25 15:50:38.000000 decorator_parser-1.0.3/src/decorator_parser/errors.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4468 2023-06-25 15:50:30.000000 decorator_parser-1.0.3/src/decorator_parser/parse.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      297 2023-06-25 15:49:06.000000 decorator_parser-1.0.3/src/decorator_parser/parse_task.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      522 2023-06-25 14:48:43.000000 decorator_parser-1.0.3/src/decorator_parser/test.py
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      240 2023-06-25 15:50:44.000000 decorator_parser-1.0.3/src/decorator_parser/utils.py
-drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 15:51:15.458257 decorator_parser-1.0.3/src/decorator_parser.egg-info/
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4339 2023-06-25 15:51:15.000000 decorator_parser-1.0.3/src/decorator_parser.egg-info/PKG-INFO
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      396 2023-06-25 15:51:15.000000 decorator_parser-1.0.3/src/decorator_parser.egg-info/SOURCES.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        1 2023-06-25 15:51:15.000000 decorator_parser-1.0.3/src/decorator_parser.egg-info/dependency_links.txt
--rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       17 2023-06-25 15:51:15.000000 decorator_parser-1.0.3/src/decorator_parser.egg-info/top_level.txt
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-26 10:31:49.026860 decorator_parser-1.0.4/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      519 2023-06-25 14:29:47.000000 decorator_parser-1.0.4/LICENSE
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4165 2023-06-26 10:31:49.026860 decorator_parser-1.0.4/PKG-INFO
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     3655 2023-06-26 10:25:15.000000 decorator_parser-1.0.4/README.md
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      587 2023-06-26 10:30:18.000000 decorator_parser-1.0.4/pyproject.toml
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       38 2023-06-26 10:31:49.026860 decorator_parser-1.0.4/setup.cfg
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-26 10:31:49.016860 decorator_parser-1.0.4/src/
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-26 10:31:49.026860 decorator_parser-1.0.4/src/decorator_parser/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-25 14:21:25.000000 decorator_parser-1.0.4/src/decorator_parser/__init__.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     1093 2023-06-25 15:50:38.000000 decorator_parser-1.0.4/src/decorator_parser/errors.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4196 2023-06-26 10:30:00.000000 decorator_parser-1.0.4/src/decorator_parser/parse.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      323 2023-06-26 10:10:32.000000 decorator_parser-1.0.4/src/decorator_parser/parse_task.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      522 2023-06-25 14:48:43.000000 decorator_parser-1.0.4/src/decorator_parser/test.py
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      240 2023-06-25 15:50:44.000000 decorator_parser-1.0.4/src/decorator_parser/utils.py
+drwxr-xr-x   0 mkostyk   (1000) mkostyk   (1000)        0 2023-06-26 10:31:49.026860 decorator_parser-1.0.4/src/decorator_parser.egg-info/
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)     4165 2023-06-26 10:31:49.000000 decorator_parser-1.0.4/src/decorator_parser.egg-info/PKG-INFO
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)      396 2023-06-26 10:31:49.000000 decorator_parser-1.0.4/src/decorator_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)        1 2023-06-26 10:31:49.000000 decorator_parser-1.0.4/src/decorator_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 mkostyk   (1000) mkostyk   (1000)       17 2023-06-26 10:31:49.000000 decorator_parser-1.0.4/src/decorator_parser.egg-info/top_level.txt
```

### Comparing `decorator_parser-1.0.3/LICENSE` & `decorator_parser-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator_parser-1.0.3/PKG-INFO` & `decorator_parser-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator_parser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -18,15 +18,16 @@
 
 ### Installation guide
 1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
 2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
 3. Run `pip install decorator-parser` in your command line
 
 ### Decorators format
-Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
+Decorator name can be any string that does not contain '@' character. If decorator
+does not satisfy this requirement `InvalidDecoratorException` will be thrown.
 
 #### Example:
 ```
 @decorator(some nice value)
 ```
 
 ### Standard decorators
```

### Comparing `decorator_parser-1.0.3/README.md` & `decorator_parser-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 ### Installation guide
 1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
 2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
 3. Run `pip install decorator-parser` in your command line
 
 ### Decorators format
-Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
+Decorator name can be any string that does not contain '@' character. If decorator
+does not satisfy this requirement `InvalidDecoratorException` will be thrown.
 
 #### Example:
 ```
 @decorator(some nice value)
 ```
 
 ### Standard decorators
```

### Comparing `decorator_parser-1.0.3/pyproject.toml` & `decorator_parser-1.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decorator_parser"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Michal Kostyk", email="m.kostyk22@gmail.com" },
 ]
 description = "Parser for text files with decorators into Python dictionaries"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `decorator_parser-1.0.3/src/decorator_parser/errors.py` & `decorator_parser-1.0.4/src/decorator_parser/errors.py`

 * *Files identical despite different names*

### Comparing `decorator_parser-1.0.3/src/decorator_parser/parse.py` & `decorator_parser-1.0.4/src/decorator_parser/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
-# Version: 1.0.3
+# Version: 1.0.4
 
 from errors import *
 from utils import *
 import re
 
 
 class Parser:
@@ -15,26 +15,22 @@
 
         self.constraints = constraints
         pass
         
 
     # Parse @global decorators
     def parse_global(self, data):
-        global_decorators = re.findall(r'(@global\-[^\s]*)', data)
+        global_decorators = re.findall(r'(@global\-[^\n]*)', data)
         if len(global_decorators) == 0:
             return data, {}
         
         # Removing decorators from data
         for gd in global_decorators:
             data = data.replace(gd, '')
         
-        # Removing @global- prefix from decorators
-        for i in range(len(global_decorators)):
-            global_decorators[i] = global_decorators[i].replace('@global-', '@')
-
         gd_text = '\n'.join(global_decorators)
         gd_result = self.create_result(gd_text, {})
 
         return data, gd_result
 
 
     # Splits file by @new decorator
@@ -52,32 +48,31 @@
 
         data = '@' + '@'.join(data.split('@')[2:])
 
         return data
 
 
     # Handles a single decorator.
-    def handle_decorator(self, data, result):
-        # Look for the first @ in the file - it is a candidate for a decorator
-        candidate = re.search(r'(@[^\n]*$)', data, re.MULTILINE)
-        if candidate is None:
-            raise DecoratorNotFoundException("No more decorators found")
-        candidate = candidate.group(0)
-        
-        # Look for a legit decorator
-        decorator = re.search(r'(@[^\s]*$)', data, re.MULTILINE)
+    def handle_decorator(self, data, result):       
+        # Look for a decorator
+        decorator = re.search(r'(@[^\n]*$)', data, re.MULTILINE)
         if decorator is None:
-            raise InvalidDecoratorException(self.original_data, candidate, "Invalid decorator")
+            raise DecoratorNotFoundException("No more decorators found")
         decorator = decorator.group(0)
 
-        # Check if decorator is the same as candidate
-        if not decorator == candidate:
-            raise InvalidDecoratorException(self.original_data, candidate, "Invalid decorator")
+        # Check if decorator is valid
+        if re.search(r'(@[^\n]*@[^\n]*$)', decorator, re.MULTILINE) is not None:
+            raise InvalidDecoratorException(self.original_data, decorator, "Invalid decorator")
         
+        is_global = re.search(r'(@global\-[^\n]*)', decorator) is not None       
         name = decorator.split('(')[0].split('@')[1]
+        if is_global:
+            # Removing global- prefix from name
+            name = name.replace('global-', '')
+
         decor_with_val = decorator # For error messages
         value = ""
 
         # Value can be put in brackets or after decorator
         try:
             value = decorator.split('(')[1].split(')')[0].strip()
         except IndexError:
```

### Comparing `decorator_parser-1.0.3/src/decorator_parser/test.py` & `decorator_parser-1.0.4/src/decorator_parser/test.py`

 * *Files identical despite different names*

### Comparing `decorator_parser-1.0.3/src/decorator_parser.egg-info/PKG-INFO` & `decorator_parser-1.0.4/src/decorator_parser.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -18,15 +18,16 @@
 
 ### Installation guide
 1. Install Python 3.7 or newer from [https://www.python.org/downloads/](https://www.python.org/downloads/)
 2. Install PIP using [this guide](https://pip.pypa.io/en/stable/installation/)
 3. Run `pip install decorator-parser` in your command line
 
 ### Decorators format
-Decorator name can be any string that does not contain '@' character or a newline character. There should be no whitespaces after the decorator name nor after its closing parenthesis. Decorator can, but does not have to end with a newline. If a decorator does not satisfy these requirements `InvalidDecoratorException` will be thrown.
+Decorator name can be any string that does not contain '@' character. If decorator
+does not satisfy this requirement `InvalidDecoratorException` will be thrown.
 
 #### Example:
 ```
 @decorator(some nice value)
 ```
 
 ### Standard decorators
```

