# Comparing `tmp/pydoclint-0.0.8.tar.gz` & `tmp/pydoclint-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.8.tar", last modified: Tue Jun  6 08:37:39 2023, max compression
+gzip compressed data, was "pydoclint-0.0.9.tar", last modified: Mon Jun 12 08:31:16 2023, max compression
```

## Comparing `pydoclint-0.0.8.tar` & `pydoclint-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-06 08:37:23.000000 pydoclint-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-06 08:37:39.376371 pydoclint-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-06-06 08:37:23.000000 pydoclint-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.368371 pydoclint-0.0.8/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 08:37:39.000000 pydoclint-0.0.8/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-06 08:37:23.000000 pydoclint-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 08:37:39.376371 pydoclint-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 08:37:23.000000 pydoclint-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:39.372371 pydoclint-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-06-06 08:37:23.000000 pydoclint-0.0.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 08:37:23.000000 pydoclint-0.0.8/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.967443 pydoclint-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-12 08:31:07.000000 pydoclint-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-06-12 08:31:16.967443 pydoclint-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-12 08:31:07.000000 pydoclint-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.963443 pydoclint-0.0.9/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.967443 pydoclint-0.0.9/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.963443 pydoclint-0.0.9/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 08:31:16.000000 pydoclint-0.0.9/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 08:31:07.000000 pydoclint-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 08:31:16.967443 pydoclint-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 08:31:07.000000 pydoclint-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:31:16.967443 pydoclint-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    33175 2023-06-12 08:31:07.000000 pydoclint-0.0.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-12 08:31:07.000000 pydoclint-0.0.9/tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.8/LICENSE` & `pydoclint-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/PKG-INFO` & `pydoclint-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.8
-Summary: A linter to check arguments in Python docstrings
+Version: 0.0.9
+Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -13,16 +13,16 @@
 
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
-[darglint](https://github.com/terrencepreilly/darglint) (another linter of the
-same purposes which is no longer maintained).
+[darglint](https://github.com/terrencepreilly/darglint) (or its maintained fork
+[darglint2](https://github.com/akaihola/darglint2)).
 
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
@@ -257,30 +257,34 @@
 
 or
 
 ```
 flake8 --style=google <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.4. `--type-hints-in-docstring` and `--type-hints-in-signature`
 
-If `True`, the type hints in the docstring and in the Python code need to
-exactly match.
+- `--type-hints-in-docstring`
+  - Shortform: `-thd`
+  - Default: `True`
+  - Meaning:
+    - If `True`, there need to be type hints in the argument list of a
+      docstring
+    - If `False`, there cannot be any type hints in the argument list of a
+      docstring
+- `--type-hints-in-signature`
+  - Shortform: `-ths`
+  - Default: `True`
+  - Meaning:
+    - If `True`, there need to be type hints in the function/method signature
+    - If `False`, there cannot be any type hints in the function/method
+      signature
 
-To turn this option on/off, do this:
-
-```
-pydoclint --check-type-hint=False <FILE_OR_FOLDER>
-```
-
-or
-
-```
-flake8 --check-type-hint=False <FILE_OR_FOLDER>
-```
+Note: if users choose `True` for both options, the type hints in the signature
+and in the docstring need to match, otherwise there will be a style violation.
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this option on/off, do this:
```

### Comparing `pydoclint-0.0.8/README.md` & `pydoclint-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
-[darglint](https://github.com/terrencepreilly/darglint) (another linter of the
-same purposes which is no longer maintained).
+[darglint](https://github.com/terrencepreilly/darglint) (or its maintained fork
+[darglint2](https://github.com/akaihola/darglint2)).
 
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
@@ -244,30 +244,34 @@
 
 or
 
 ```
 flake8 --style=google <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.4. `--type-hints-in-docstring` and `--type-hints-in-signature`
 
-If `True`, the type hints in the docstring and in the Python code need to
-exactly match.
+- `--type-hints-in-docstring`
+  - Shortform: `-thd`
+  - Default: `True`
+  - Meaning:
+    - If `True`, there need to be type hints in the argument list of a
+      docstring
+    - If `False`, there cannot be any type hints in the argument list of a
+      docstring
+- `--type-hints-in-signature`
+  - Shortform: `-ths`
+  - Default: `True`
+  - Meaning:
+    - If `True`, there need to be type hints in the function/method signature
+    - If `False`, there cannot be any type hints in the function/method
+      signature
 
-To turn this option on/off, do this:
-
-```
-pydoclint --check-type-hint=False <FILE_OR_FOLDER>
-```
-
-or
-
-```
-flake8 --check-type-hint=False <FILE_OR_FOLDER>
-```
+Note: if users choose `True` for both options, the type hints in the signature
+and in the docstring need to match, otherwise there will be a style violation.
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this option on/off, do this:
```

### Comparing `pydoclint-0.0.8/pydoclint/flake8_entry.py` & `pydoclint-0.0.9/pydoclint/flake8_entry.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,28 @@
             '--style',
             action='store',
             default='numpy',
             parse_from_config=True,
             help='Which style of docstring is your code base using',
         )
         parser.add_option(
-            '-th',
-            '--check-type-hint',
+            '-ths',
+            '--type-hints-in-signature',
             action='store',
             default='True',
             parse_from_config=True,
-            help='Whether to check type hints in the docstring',
+            help='Whether to require type hints in function signatures',
+        )
+        parser.add_option(
+            '-thd',
+            '--type-hints-in-docstring',
+            action='store',
+            default='True',
+            parse_from_config=True,
+            help='Whether to require type hints in the argument list in docstrings',
         )
         parser.add_option(
             '-ao',
             '--check-arg-order',
             action='store',
             default='True',
             parse_from_config=True,
@@ -77,29 +85,37 @@
                 ' the function body does not have a "return" statement and'
                 ' the return type annotation is "-> None".'
             ),
         )
 
     @classmethod
     def parse_options(cls, options):  # noqa: D102
-        cls.check_type_hint = options.check_type_hint
+        cls.type_hints_in_signature = options.type_hints_in_signature
+        cls.type_hints_in_docstring = options.type_hints_in_docstring
         cls.check_arg_order = options.check_arg_order
         cls.skip_checking_short_docstrings = (
             options.skip_checking_short_docstrings
         )
         cls.skip_checking_raises = options.skip_checking_raises
         cls.allow_init_docstring = options.allow_init_docstring
         cls.require_return_section_when_returning_none = (
             options.require_return_section_when_returning_none
         )
         cls.style = options.style
 
     def run(self) -> Generator[Tuple[int, int, str, Any], None, None]:
         """Run the linter and yield the violation information"""
-        checkTypeHint = self._bool('--check-type-hint', self.check_type_hint)
+        typeHintsInSignature = self._bool(
+            '--type-hints-in-signature',
+            self.type_hints_in_signature,
+        )
+        typeHintsInDocstring = self._bool(
+            '--type-hints-in-docstring',
+            self.type_hints_in_docstring,
+        )
         checkArgOrder = self._bool('--check-arg-order', self.check_arg_order)
         skipCheckingShortDocstrings = self._bool(
             '--skip-checking-short-docstrings',
             self.skip_checking_short_docstrings,
         )
         skipCheckingRaises = self._bool(
             '--skip-checking-raises',
@@ -116,15 +132,16 @@
 
         if self.style not in {'numpy', 'google'}:
             raise ValueError(
                 'Invalid value for "--style": must be "numpy" or "google"'
             )
 
         v = Visitor(
-            checkTypeHint=checkTypeHint,
+            typeHintsInSignature=typeHintsInSignature,
+            typeHintsInDocstring=typeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
             requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
             style=self.style,
         )
```

### Comparing `pydoclint-0.0.8/pydoclint/main.py` & `pydoclint-0.0.9/pydoclint/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,20 +64,28 @@
     type=str,
     show_default=True,
     default='numpy',
     callback=validateStyleValue,
     help='',
 )
 @click.option(
-    '-th',
-    '--check-type-hint',
+    '-ths',
+    '--type-hints-in-signature',
     type=bool,
     show_default=True,
     default=True,
-    help='Whether to check type hints in docstrings',
+    help='Whether to require type hints in function signatures',
+)
+@click.option(
+    '-thd',
+    '--type-hints-in-docstring',
+    type=bool,
+    show_default=True,
+    default=True,
+    help='Whether to require type hints in the argument list in docstrings',
 )
 @click.option(
     '-ao',
     '--check-arg-order',
     type=bool,
     show_default=True,
     default=True,
@@ -154,21 +162,22 @@
 def main(  # noqa: C901
         ctx: click.Context,
         quiet: bool,
         exclude: str,
         style: str,
         src: Optional[str],
         paths: Tuple[str, ...],
-        check_type_hint: bool,
+        type_hints_in_signature: bool,
+        type_hints_in_docstring: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
         allow_init_docstring: bool,
         require_return_section_when_returning_none: bool,
-        config: Optional[str],
+        config: Optional[str],  # don't remove it b/c it's required by `click`
 ) -> None:
     """Command-line entry point of pydoclint"""
     ctx.ensure_object(dict)
 
     if paths and src is not None:
         click.echo(
             main.get_usage(ctx)
@@ -185,15 +194,16 @@
         ctx.exit(1)
 
     violationsInAllFiles: Dict[str, List[Violation]] = _checkPaths(
         quiet=quiet,
         exclude=exclude,
         style=style,
         paths=paths,
-        checkTypeHint=check_type_hint,
+        typeHintsInSignature=type_hints_in_signature,
+        typeHintsInDocstring=type_hints_in_docstring,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
         allowInitDocstring=allow_init_docstring,
         requireReturnSectionWhenReturningNone=require_return_section_when_returning_none,
     )
 
@@ -239,15 +249,16 @@
 
         ctx.exit(0)
 
 
 def _checkPaths(
         paths: Tuple[str, ...],
         style: str = 'numpy',
-        checkTypeHint: bool = True,
+        typeHintsInSignature: bool = True,
+        typeHintsInDocstring: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
         requireReturnSectionWhenReturningNone: bool = False,
         quiet: bool = False,
         exclude: str = '',
@@ -279,43 +290,46 @@
             click.echo(
                 click.style(filename, fg='cyan', bold=True), err=echoAsError
             )
 
         violationsInThisFile: List[Violation] = _checkFile(
             filename,
             style=style,
-            checkTypeHint=checkTypeHint,
+            typeHintsInSignature=typeHintsInSignature,
+            typeHintsInDocstring=typeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
             requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
         )
         allViolations[filename.as_posix()] = violationsInThisFile
 
     return allViolations
 
 
 def _checkFile(
         filename: Path,
         style: str = 'numpy',
-        checkTypeHint: bool = True,
+        typeHintsInSignature: bool = True,
+        typeHintsInDocstring: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
         requireReturnSectionWhenReturningNone: bool = False,
 ) -> List[Violation]:
     with open(filename, encoding='utf8') as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
         style=style,
-        checkTypeHint=checkTypeHint,
+        typeHintsInSignature=typeHintsInSignature,
+        typeHintsInDocstring=typeHintsInDocstring,
         checkArgOrder=checkArgOrder,
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
         skipCheckingRaises=skipCheckingRaises,
         allowInitDocstring=allowInitDocstring,
         requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
     )
     visitor.visit(tree)
```

### Comparing `pydoclint-0.0.8/pydoclint/parse_config.py` & `pydoclint-0.0.9/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/annotation.py` & `pydoclint-0.0.9/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/arg.py` & `pydoclint-0.0.9/pydoclint/utils/arg.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,14 +52,26 @@
     def __hash__(self) -> int:
         return hash((self.name, self._stripQuotes(self.typeHint)))
 
     def nameEquals(self, other: 'Arg') -> bool:
         """More lenient equality: only compare names"""
         return self.name == other.name
 
+    def hasTypeHint(self) -> bool:
+        """Check whether this arg has type hint"""
+        return self.typeHint != ''
+
+    def isStarArg(self) -> bool:
+        """Check whether this arg is a star arg (such as *args, **kwargs)"""
+        return self.name.startswith('*')
+
+    def notStarArg(self) -> bool:
+        """Check whether this arg is not a star arg (*args, **kwargs)"""
+        return not self.isStarArg()
+
     @classmethod
     def fromNumpydocParam(cls, param: Parameter) -> 'Arg':
         """Construct an Arg object from a Numpydoc Parameter object"""
         return Arg(name=param.name, typeHint=param.type)
 
     @classmethod
     def fromGoogleParsedParam(cls, param: DocstringParam) -> 'Arg':
@@ -201,7 +213,29 @@
                 verdict = set(self_names) == set(other_names)
 
         return verdict  # noqa: R504
 
     def subtract(self, other: 'ArgList') -> Set[Arg]:
         """Find the args that are in this object but not in `other`."""
         return set(self.infoList) - set(other.infoList)
+
+    def noTypeHints(self) -> bool:
+        """Check whether none of the args have type hints"""
+        return not self.hasTypeHintInAnyArg()
+
+    def hasTypeHintInAnyArg(self) -> bool:
+        """
+        Check whether any arg has a type hint.
+
+        Start arguments (such as `*args` or `**kwargs`) are excluded because
+        they don't need to have type hints.
+        """
+        return any(_.hasTypeHint() for _ in self.infoList if _.notStarArg())
+
+    def hasTypeHintInAllArgs(self) -> bool:
+        """
+        Check whether all args have a type hint.
+
+        Start arguments (such as `*args` or `**kwargs`) are excluded because
+        they don't need to have type hints.
+        """
+        return all(_.hasTypeHint() for _ in self.infoList if _.notStarArg())
```

### Comparing `pydoclint-0.0.8/pydoclint/utils/astTypes.py` & `pydoclint-0.0.9/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/doc.py` & `pydoclint-0.0.9/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/generic.py` & `pydoclint-0.0.9/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.9/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/unparser.py` & `pydoclint-0.0.9/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/utils/violation.py` & `pydoclint-0.0.9/pydoclint/utils/violation.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,20 @@
     102: 'Docstring contains more arguments than in function signature.',
     103: (  # noqa: PAR001
         'Docstring arguments are different from function arguments.'
         ' (Or could be other formatting issues: https://github.com/jsh9/pydoclint#notes-on-doc103 ).'
     ),
     104: 'Arguments are the same in the docstring and the function signature, but are in a different order.',
     105: 'Argument names match, but type hints do not match',
+    106: 'The option `--type-hints-in-signature` is `True` but there are no type hints in the signature',
+    107: 'The option `--type-hints-in-signature` is `True` but not all args in the signature have type hints',
+    108: 'The option `--type-hints-in-signature` is `False` but there are type hints in the signature',
+    109: 'The option `--type-hints-in-docstring` is `True` but there are no type hints in the docstring arg list',
+    110: 'The option `--type-hints-in-docstring` is `True` but not all args in the docstring arg list have type hints',
+    111: 'The option `--type-hints-in-docstring` is `False` but there are type hints in the docstring arg list',
 
     201: 'does not have a return section in docstring',
     202: 'has a return section in docstring, but there are no return statements or annotations',
 
     301: '__init__() should not have a docstring; please combine it with the docstring of the class',
     302: 'The class docstring does not need a "Returns" section, because __init__() cannot return anything',
     303: 'The __init__() docstring does not need a "Returns" section, because it cannot return anything',
```

### Comparing `pydoclint-0.0.8/pydoclint/utils/walk.py` & `pydoclint-0.0.9/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/pydoclint/visitor.py` & `pydoclint-0.0.9/pydoclint/visitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,23 +27,25 @@
 
 class Visitor(ast.NodeVisitor):
     """A class to recursively visit all the nodes in a parsed module"""
 
     def __init__(
             self,
             style: str = 'numpy',
-            checkTypeHint: bool = True,
+            typeHintsInSignature: bool = True,
+            typeHintsInDocstring: bool = True,
             checkArgOrder: bool = True,
             skipCheckingShortDocstrings: bool = True,
             skipCheckingRaises: bool = False,
             allowInitDocstring: bool = False,
             requireReturnSectionWhenReturningNone: bool = False,
     ) -> None:
         self.style: str = style
-        self.checkTypeHint: bool = checkTypeHint
+        self.typeHintsInSignature: bool = typeHintsInSignature
+        self.typeHintsInDocstring: bool = typeHintsInDocstring
         self.checkArgOrder: bool = checkArgOrder
         self.skipCheckingShortDocstrings: bool = skipCheckingShortDocstrings
         self.skipCheckingRaises: bool = skipCheckingRaises
         self.allowInitDocstring: bool = allowInitDocstring
         self.requireReturnSectionWhenReturningNone: bool = (
             requireReturnSectionWhenReturningNone
         )
@@ -311,45 +313,70 @@
                 astArgList = astArgList[1:]  # no need to document self/cls
 
         lineNum: int = node.lineno
         v101 = Violation(code=101, line=lineNum, msgPrefix=msgPrefix)
         v102 = Violation(code=102, line=lineNum, msgPrefix=msgPrefix)
         v104 = Violation(code=104, line=lineNum, msgPrefix=msgPrefix)
         v105 = Violation(code=105, line=lineNum, msgPrefix=msgPrefix)
+        v106 = Violation(code=106, line=lineNum, msgPrefix=msgPrefix)
+        v107 = Violation(code=107, line=lineNum, msgPrefix=msgPrefix)
+        v108 = Violation(code=108, line=lineNum, msgPrefix=msgPrefix)
+        v109 = Violation(code=109, line=lineNum, msgPrefix=msgPrefix)
+        v110 = Violation(code=110, line=lineNum, msgPrefix=msgPrefix)
+        v111 = Violation(code=111, line=lineNum, msgPrefix=msgPrefix)
 
-        docArgs = doc.argList
-        funcArgs = ArgList([Arg.fromAstArg(_) for _ in astArgList])
+        docArgs: ArgList = doc.argList
+        funcArgs: ArgList = ArgList([Arg.fromAstArg(_) for _ in astArgList])
 
         if docArgs.length == 0 and funcArgs.length == 0:
             return []
 
         violations: List[Violation] = []
         if docArgs.length < funcArgs.length:
             violations.append(v101)
 
         if docArgs.length > funcArgs.length:
             violations.append(v102)
 
+        if self.typeHintsInSignature and funcArgs.noTypeHints():
+            violations.append(v106)
+
+        if self.typeHintsInSignature and not funcArgs.hasTypeHintInAllArgs():
+            violations.append(v107)
+
+        if not self.typeHintsInSignature and funcArgs.hasTypeHintInAnyArg():
+            violations.append(v108)
+
+        if self.typeHintsInDocstring and docArgs.noTypeHints():
+            violations.append(v109)
+
+        if self.typeHintsInDocstring and not docArgs.hasTypeHintInAllArgs():
+            violations.append(v110)
+
+        if not self.typeHintsInDocstring and docArgs.hasTypeHintInAnyArg():
+            violations.append(v111)
+
         if not docArgs.equals(
             funcArgs,
-            checkTypeHint=self.checkTypeHint,
+            checkTypeHint=True,
             orderMatters=self.checkArgOrder,
         ):
             if docArgs.equals(
                 funcArgs,
-                checkTypeHint=self.checkTypeHint,
+                checkTypeHint=True,
                 orderMatters=False,
             ):
                 violations.append(v104)
             elif docArgs.equals(
                 funcArgs,
                 checkTypeHint=False,
                 orderMatters=self.checkArgOrder,
             ):
-                violations.append(v105)
+                if self.typeHintsInSignature and self.typeHintsInDocstring:
+                    violations.append(v105)
             elif docArgs.equals(
                 funcArgs,
                 checkTypeHint=False,
                 orderMatters=False,
             ):
                 violations.append(v104)
                 violations.append(v105)
```

### Comparing `pydoclint-0.0.8/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.9/pydoclint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.8
-Summary: A linter to check arguments in Python docstrings
+Version: 0.0.9
+Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -13,16 +13,16 @@
 
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
-[darglint](https://github.com/terrencepreilly/darglint) (another linter of the
-same purposes which is no longer maintained).
+[darglint](https://github.com/terrencepreilly/darglint) (or its maintained fork
+[darglint2](https://github.com/akaihola/darglint2)).
 
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
@@ -257,30 +257,34 @@
 
 or
 
 ```
 flake8 --style=google <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.4. `--type-hints-in-docstring` and `--type-hints-in-signature`
 
-If `True`, the type hints in the docstring and in the Python code need to
-exactly match.
+- `--type-hints-in-docstring`
+  - Shortform: `-thd`
+  - Default: `True`
+  - Meaning:
+    - If `True`, there need to be type hints in the argument list of a
+      docstring
+    - If `False`, there cannot be any type hints in the argument list of a
+      docstring
+- `--type-hints-in-signature`
+  - Shortform: `-ths`
+  - Default: `True`
+  - Meaning:
+    - If `True`, there need to be type hints in the function/method signature
+    - If `False`, there cannot be any type hints in the function/method
+      signature
 
-To turn this option on/off, do this:
-
-```
-pydoclint --check-type-hint=False <FILE_OR_FOLDER>
-```
-
-or
-
-```
-flake8 --check-type-hint=False <FILE_OR_FOLDER>
-```
+Note: if users choose `True` for both options, the type hints in the signature
+and in the docstring need to match, otherwise there will be a style violation.
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
 To turn this option on/off, do this:
```

### Comparing `pydoclint-0.0.8/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.9/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.8/setup.cfg` & `pydoclint-0.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = pydoclint
-version = 0.0.8
-description = A linter to check arguments in Python docstrings
+version = 0.0.9
+description = A Python docstring linter that checks arguments, returns, yields, and raises sections
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `pydoclint-0.0.8/tests/test_main.py` & `pydoclint-0.0.9/tests/test_main.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,64 +7,27 @@
 
 from pydoclint.main import _checkFile
 
 THIS_DIR = Path(__file__).parent
 DATA_DIR = THIS_DIR / 'data'
 
 
-expectedViolations_True_True = [
-    'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
-    'the docstring: [arg1: str, arg2: list[int]].',
-    'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
-    'function signature: [arg1: int].',
-    'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
-    'the docstring: [arg2: float | int | None].',
-    'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
-    'function signature: [arg3: Optional[Union[float, int, str]]].',
-    'DOC104: Method `MyClass.func4`: Arguments are the same in the docstring and '
-    'the function signature, but are in a different order. ',
-    'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
-    'match ',
-    'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
-    'the function signature, but are in a different order. ',
-    'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
-    'match ',
-    'DOC101: Function `func72`: Docstring contains fewer arguments than in '
-    'function signature. ',
-    'DOC103: Function `func72`: Docstring arguments are different from function '
-    'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
-    'docstring: [arg3: list, arg4: tuple, arg5: dict].',
-]
-
-expectedViolations_False_True = [
+expectedViolations_True = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC109: Method `MyClass.func1_3`: The option `--type-hints-in-docstring` is `True` '
+    'but there are no type hints in the docstring arg list ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
+    'DOC106: Method `MyClass.func1_6`: The option `--type-hints-in-signature` is `True` '
+    'but there are no type hints in the signature ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
@@ -75,33 +38,41 @@
     'function signature. ',
     'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC104: Method `MyClass.func4`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
+    'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not match ',
     'DOC104: Method `MyClass.func6`: Arguments are the same in the docstring and '
     'the function signature, but are in a different order. ',
+    'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC109: Function `func72`: The option `--type-hints-in-docstring` is `True` '
+    'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
-expectedViolations_True_False = [
+expectedViolations_False = [
     'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC109: Method `MyClass.func1_3`: The option `--type-hints-in-docstring` is `True` '
+    'but there are no type hints in the docstring arg list ',
     'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
     'the docstring: [arg1: str, arg2: list[int]].',
     'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
     'function signature. ',
+    'DOC106: Method `MyClass.func1_6`: The option `--type-hints-in-signature` is `True` '
+    'but there are no type hints in the signature ',
     'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
     'function arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
     'function signature: [arg1: int].',
     'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
     'function signature. ',
     'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
@@ -116,101 +87,52 @@
     'function signature: [arg3: Optional[Union[float, int, str]]].',
     'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
     'match ',
     'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
     'match ',
     'DOC101: Function `func72`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC109: Function `func72`: The option `--type-hints-in-docstring` is `True` '
+    'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func72`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg3: list, arg4: tuple, arg5: dict].',
 ]
 
-expectedViolations_False_False = [
-    'DOC101: Method `MyClass.func1_3`: Docstring contains fewer arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func1_3`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
-    'the docstring: [arg1: str, arg2: list[int]].',
-    'DOC102: Method `MyClass.func1_6`: Docstring contains more arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func1_6`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
-    'function signature: [arg1: int].',
-    'DOC101: Method `MyClass.func2`: Docstring contains fewer arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func2`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in '
-    'the docstring: [arg2: float | int | None].',
-    'DOC102: Method `MyClass.func3`: Docstring contains more arguments than in '
-    'function signature. ',
-    'DOC103: Method `MyClass.func3`: Docstring arguments are different from '
-    'function arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the docstring but not in the '
-    'function signature: [arg3: Optional[Union[float, int, str]]].',
-    'DOC101: Function `func72`: Docstring contains fewer arguments than in '
-    'function signature. ',
-    'DOC103: Function `func72`: Docstring arguments are different from function '
-    'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
-    'docstring: [arg3: list, arg4: tuple, arg5: dict].',
-]
-
-expectedViolationsLookup: Dict[str, List[str]] = {
-    'true_true': expectedViolations_True_True,
-    'true_false': expectedViolations_True_False,
-    'false_true': expectedViolations_False_True,
-    'false_false': expectedViolations_False_False,
-}
-
-optionDictLookup: Dict[str, Dict[str, bool]] = {
-    'true_true': {'checkTypeHint': True, 'checkArgOrder': True},
-    'true_false': {'checkTypeHint': True, 'checkArgOrder': False},
-    'false_true': {'checkTypeHint': False, 'checkArgOrder': True},
-    'false_false': {'checkTypeHint': False, 'checkArgOrder': False},
+expectedViolationsLookup: Dict[bool, List[str]] = {
+    True: expectedViolations_True,
+    False: expectedViolations_False,
 }
 
-options = [
-    'true_true',
-    'true_false',
-    'false_true',
-    'false_false',
-]
-
 
 @pytest.mark.parametrize(
-    'style, filename, option',
+    'style, filename, checkArgOrder',
     list(
         itertools.product(
             ['numpy', 'google'],
             ['function.py', 'classmethod.py', 'method.py', 'staticmethod.py'],
-            options,
+            [True, False],
         ),
     ),
 )
 def testArguments(
         style: str,
         filename: str,
-        option: str,
+        checkArgOrder: str,
 ) -> None:
-    optionDict: Dict[str, bool] = optionDictLookup[option]
-    expectedViolations: List[str] = expectedViolationsLookup[option]
+    expectedViolations: List[str] = expectedViolationsLookup[checkArgOrder]
 
     expectedViolationsCopy = copy.deepcopy(expectedViolations)
     if filename == 'function.py':
         _tweakViolationMsgForFunctions(expectedViolationsCopy)
 
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/args/{filename}',
-        checkTypeHint=optionDict['checkTypeHint'],
-        checkArgOrder=optionDict['checkArgOrder'],
+        checkArgOrder=checkArgOrder,
         style=style,
     )
     assert list(map(str, violations)) == expectedViolationsCopy
 
 
 @pytest.mark.parametrize(
     'style, filename',
@@ -258,58 +180,79 @@
 def _tweakViolationMsgForFunctions(expectedViolationsCopy: List[str]) -> None:
     for i in range(len(expectedViolationsCopy)):
         expectedViolationsCopy[i] = expectedViolationsCopy[i].replace(
             'Method `MyClass.', 'Function `'
         )
 
 
-expected_True = [
+expected_skipCheckingShortDocstrings_True = [
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC106: Function `func3`: The option `--type-hints-in-signature` is `True` '
+    'but there are no type hints in the signature ',
+    'DOC107: Function `func3`: The option `--type-hints-in-signature` is `True` '
+    'but not all args in the signature have type hints ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
     'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
     'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
     'the function signature: [var1: int, var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
-expected_False = [
+expected_skipCheckingShortDocstrings_False = [
     'DOC101: Function `func1`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC106: Function `func1`: The option `--type-hints-in-signature` is `True` '
+    'but there are no type hints in the signature ',
+    'DOC107: Function `func1`: The option `--type-hints-in-signature` is `True` '
+    'but not all args in the signature have type hints ',
+    'DOC109: Function `func1`: The option `--type-hints-in-docstring` is `True` '
+    'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func1`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
-    'docstring: [arg1: , arg2: , arg3: ].',
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
+    'function signature but not in the docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func1` does not have a return section in docstring ',
     'DOC101: Function `func2`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC106: Function `func2`: The option `--type-hints-in-signature` is `True` '
+    'but there are no type hints in the signature ',
+    'DOC107: Function `func2`: The option `--type-hints-in-signature` is `True` '
+    'but not all args in the signature have type hints ',
+    'DOC109: Function `func2`: The option `--type-hints-in-docstring` is `True` '
+    'but there are no type hints in the docstring arg list ',
     'DOC103: Function `func2`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
-    'docstring: [arg1: , arg2: , arg3: ].',
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
+    'function signature but not in the docstring: [arg1: , arg2: , arg3: ].',
     'DOC201: Function `func2` does not have a return section in docstring ',
     'DOC101: Function `func3`: Docstring contains fewer arguments than in '
     'function signature. ',
+    'DOC106: Function `func3`: The option `--type-hints-in-signature` is `True` '
+    'but there are no type hints in the signature ',
+    'DOC107: Function `func3`: The option `--type-hints-in-signature` is `True` '
+    'but not all args in the signature have type hints ',
     'DOC103: Function `func3`: Docstring arguments are different from function '
     'arguments. (Or could be other formatting issues: '
-    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
-    'docstring: [arg1: , arg2: , arg3: ]. Arguments in the docstring but not in '
-    'the function signature: [var1: int, var2: str].',
+    'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the '
+    'function signature but not in the docstring: [arg1: , arg2: , arg3: ]. '
+    'Arguments in the docstring but not in the function signature: [var1: int, '
+    'var2: str].',
     'DOC201: Function `func3` does not have a return section in docstring ',
 ]
 
 
 @pytest.mark.parametrize(
     'style, skipCheckingShortDocstrings, expected',
     [
-        ('numpy', True, expected_True),
-        ('numpy', False, expected_False),
-        ('google', True, expected_True),
-        ('google', False, expected_False),
+        ('numpy', True, expected_skipCheckingShortDocstrings_True),
+        ('numpy', False, expected_skipCheckingShortDocstrings_False),
+        ('google', True, expected_skipCheckingShortDocstrings_True),
+        ('google', False, expected_skipCheckingShortDocstrings_False),
     ],
 )
 def testSkipCheckingShortDocstrings(
         style: str,
         skipCheckingShortDocstrings: bool,
         expected: List[str],
 ) -> None:
@@ -426,14 +369,16 @@
         [False, True],
     ),
 )
 def testRaises(style: str, skipRaisesCheck: bool) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/raises/cases.py',
         skipCheckingRaises=skipRaisesCheck,
+        typeHintsInSignature=False,
+        typeHintsInDocstring=False,
         style=style,
     )
     expected0 = [
         'DOC501: Method `B.func1` has "raise" statements, but the docstring does not '
         'have a "Raises" section ',
         'DOC502: Method `B.func5` has a "Raises" section in the docstring, but there '
         'are not "raise" statements in the body ',
@@ -448,19 +393,23 @@
 @pytest.mark.parametrize('style', ['numpy', 'google'])
 def testStarsInArgumentList(style: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/star_args/cases.py',
         style=style,
     )
     expected = [
+        'DOC110: Function `func2`: The option `--type-hints-in-docstring` is `True` '
+        'but not all args in the docstring arg list have type hints ',
         'DOC103: Function `func2`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
         'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [**kwargs: ]. Arguments in the docstring but not in the function '
         'signature: [kwargs: ].',
+        'DOC110: Function `func4`: The option `--type-hints-in-docstring` is `True` '
+        'but not all args in the docstring arg list have type hints ',
         'DOC103: Function `func4`: Docstring arguments are different from function '
         'arguments. (Or could be other formatting issues: '
         'https://github.com/jsh9/pydoclint#notes-on-doc103 ). Arguments in the function signature but not in the '
         'docstring: [*args: ]. Arguments in the docstring but not in the function '
         'signature: [args: ].',
         'DOC101: Function `func6`: Docstring contains fewer arguments than in '
         'function signature. ',
@@ -490,14 +439,16 @@
     ]
     assert list(map(str, violations)) == expected
 
 
 def testParsingErrors_numpy() -> None:
     violations = _checkFile(
         filename=DATA_DIR / 'numpy/parsing_errors/cases.py',
+        typeHintsInDocstring=False,
+        typeHintsInSignature=False,
         style='numpy',
     )
     expected = [
         'DOC001: Function/method `__init__`: Potential formatting errors in '
         'docstring. Error message: The section Parameters appears twice in  Some '
         'class  Parameters ----------     arg1     arg2  Parameters ----------     '
         'arg3     arg4'
@@ -549,31 +500,162 @@
         style=style,
         skipCheckingShortDocstrings=True,
     )
     expected = []
     assert list(map(str, violations)) == expected
 
 
-def testPlayground() -> None:
-    """
-    This is a placeholder test for testing the `playground.py` file.
-
-    When you want to quickly test something, you can add contents into
-    tests/data/playground.py and run this test function.
-    """
+@pytest.mark.parametrize(
+    'style, typeHintsInDocstring, typeHintsInSignature',
+    itertools.product(
+        ['numpy', 'google'],
+        [False, True],
+        [False, True],
+    ),
+)
+def testTypeHintChecking(
+        style: str,
+        typeHintsInDocstring: bool,
+        typeHintsInSignature: bool,
+) -> None:
     violations = _checkFile(
-        filename=DATA_DIR / 'playground.py',
-        style='google',
+        filename=DATA_DIR / f'{style}/type_hints/cases.py',
+        style=style,
+        typeHintsInDocstring=typeHintsInDocstring,
+        typeHintsInSignature=typeHintsInSignature,
     )
-    expected = []
+
+    expected_lookup = {
+        (False, False): [
+            'DOC108: Method `MyClass.func2`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC111: Method `MyClass.func3`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC108: Method `MyClass.func4`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC111: Method `MyClass.func4`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC108: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC111: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC108: Method `MyClass.func6`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC111: Method `MyClass.func6`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC108: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC111: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+        ],
+        (False, True): [
+            'DOC106: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
+            '`True` but there are no type hints in the signature ',
+            'DOC107: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC106: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
+            '`True` but there are no type hints in the signature ',
+            'DOC107: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC111: Method `MyClass.func3`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC111: Method `MyClass.func4`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC107: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC111: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC111: Method `MyClass.func6`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+            'DOC107: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC111: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            '`False` but there are type hints in the docstring arg list ',
+        ],
+        (True, False): [
+            'DOC109: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            '`True` but there are no type hints in the docstring arg list ',
+            'DOC110: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+            'DOC108: Method `MyClass.func2`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC109: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            '`True` but there are no type hints in the docstring arg list ',
+            'DOC110: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+            'DOC108: Method `MyClass.func4`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC108: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC110: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+            'DOC108: Method `MyClass.func6`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC108: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
+            '`False` but there are type hints in the signature ',
+            'DOC110: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+        ],
+        (True, True): [
+            'DOC106: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
+            '`True` but there are no type hints in the signature ',
+            'DOC107: Method `MyClass.func1`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC109: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            '`True` but there are no type hints in the docstring arg list ',
+            'DOC110: Method `MyClass.func1`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+            'DOC109: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            '`True` but there are no type hints in the docstring arg list ',
+            'DOC110: Method `MyClass.func2`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+            'DOC105: Method `MyClass.func2`: Argument names match, but type hints do not '
+            'match ',
+            'DOC106: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
+            '`True` but there are no type hints in the signature ',
+            'DOC107: Method `MyClass.func3`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC105: Method `MyClass.func3`: Argument names match, but type hints do not '
+            'match ',
+            'DOC107: Method `MyClass.func5`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC110: Method `MyClass.func5`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+            'DOC105: Method `MyClass.func5`: Argument names match, but type hints do not '
+            'match ',
+            'DOC105: Method `MyClass.func6`: Argument names match, but type hints do not '
+            'match ',
+            'DOC107: Method `MyClass.func7`: The option `--type-hints-in-signature` is '
+            '`True` but not all args in the signature have type hints ',
+            'DOC110: Method `MyClass.func7`: The option `--type-hints-in-docstring` is '
+            '`True` but not all args in the docstring arg list have type hints ',
+        ],
+    }
+
+    expected = expected_lookup[(typeHintsInDocstring, typeHintsInSignature)]
     assert list(map(str, violations)) == expected
 
 
 def testNonAscii() -> None:
     """Don't crash on non ASCII arguments."""
     violations = _checkFile(
         filename=DATA_DIR / 'common/non_ascii/non_ascii.py',
         style='numpy',
         skipCheckingShortDocstrings=False,
     )
     expected = []
     assert list(map(str, violations)) == expected
+
+
+def testPlayground() -> None:
+    """
+    This is a placeholder test for testing the `playground.py` file.
+
+    When you want to quickly test something, you can add contents into
+    tests/data/playground.py and run this test function.
+    """
+    violations = _checkFile(
+        filename=DATA_DIR / 'playground.py',
+        style='google',
+    )
+    expected = []
+    assert list(map(str, violations)) == expected
```

### Comparing `pydoclint-0.0.8/tests/test_parse_config.py` & `pydoclint-0.0.9/tests/test_parse_config.py`

 * *Files identical despite different names*

