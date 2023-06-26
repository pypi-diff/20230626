# Comparing `tmp/beku_stackabletech-0.0.6-py3-none-any.whl.zip` & `tmp/beku_stackabletech-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,20 @@
-Zip file size: 7459 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       43 b- defN 23-Feb-19 16:57 beku/__init__.py
+Zip file size: 14723 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx       43 b- defN 23-Jun-23 15:42 beku/__init__.py
 -rw-rw-r--  2.0 unx       79 b- defN 23-Feb-19 16:46 beku/__main__.py
--rw-rw-r--  2.0 unx     2103 b- defN 23-Jun-23 14:53 beku/main.py
--rw-rw-r--  2.0 unx     7403 b- defN 23-Jun-23 14:53 beku/testsuite.py
--rw-rw-r--  2.0 unx      105 b- defN 23-Jun-23 14:54 beku/version.py
+-rw-rw-r--  2.0 unx    15694 b- defN 23-Jun-26 05:49 beku/kuttl.py
+-rw-rw-r--  2.0 unx     2370 b- defN 23-Jun-26 05:49 beku/main.py
+-rw-rw-r--  2.0 unx     7397 b- defN 23-Jun-23 15:42 beku/testsuite.py
+-rw-rw-r--  2.0 unx      105 b- defN 23-Jun-26 05:50 beku/version.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-26 05:49 beku/test/__init__.py
+-rw-rw-r--  2.0 unx    10548 b- defN 23-Jun-26 05:49 beku/test/test_render_from_stream.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-23 15:02 test/__init__.py
+-rw-rw-r--  2.0 unx     9050 b- defN 23-Jun-25 12:18 test/test_reneder_from_stream.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-23 09:39 tests/__init__.py
--rw-rw-r--  2.0 unx     1430 b- defN 23-Jun-23 14:45 tests/testsuite.py
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-23 14:55 beku_stackabletech-0.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-23 14:55 beku_stackabletech-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 14:55 beku_stackabletech-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       40 b- defN 23-Jun-23 14:55 beku_stackabletech-0.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-23 14:55 beku_stackabletech-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1049 b- defN 23-Jun-23 14:55 beku_stackabletech-0.0.6.dist-info/RECORD
-13 files, 14842 bytes uncompressed, 5697 bytes compressed:  61.6%
+-rw-rw-r--  2.0 unx     1425 b- defN 23-Jun-24 06:37 tests/testsuite.py
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1410 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       40 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1447 b- defN 23-Jun-26 05:54 beku_stackabletech-0.0.7.dist-info/RECORD
+18 files, 50774 bytes uncompressed, 12345 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -1,40 +1,55 @@
 Filename: beku/__init__.py
 Comment: 
 
 Filename: beku/__main__.py
 Comment: 
 
+Filename: beku/kuttl.py
+Comment: 
+
 Filename: beku/main.py
 Comment: 
 
 Filename: beku/testsuite.py
 Comment: 
 
 Filename: beku/version.py
 Comment: 
 
+Filename: beku/test/__init__.py
+Comment: 
+
+Filename: beku/test/test_render_from_stream.py
+Comment: 
+
+Filename: test/__init__.py
+Comment: 
+
+Filename: test/test_reneder_from_stream.py
+Comment: 
+
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/testsuite.py
 Comment: 
 
-Filename: beku_stackabletech-0.0.6.dist-info/LICENSE
+Filename: beku_stackabletech-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: beku_stackabletech-0.0.6.dist-info/METADATA
+Filename: beku_stackabletech-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: beku_stackabletech-0.0.6.dist-info/WHEEL
+Filename: beku_stackabletech-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: beku_stackabletech-0.0.6.dist-info/entry_points.txt
+Filename: beku_stackabletech-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: beku_stackabletech-0.0.6.dist-info/top_level.txt
+Filename: beku_stackabletech-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: beku_stackabletech-0.0.6.dist-info/RECORD
+Filename: beku_stackabletech-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beku/main.py

```diff
@@ -1,13 +1,14 @@
 """Main entry point."""
+import logging
 from argparse import ArgumentParser, Namespace
 from os import path
-import logging
+
+from beku.kuttl import renderer_from_file, expand
 from .version import __version__
-from .testsuite import TestSuite
 
 
 def parse_cli_args() -> Namespace:
     """Parse command line args."""
     parser = ArgumentParser(
         description="Kuttl test expander for the Stackable Data Platform")
     parser.add_argument(
@@ -58,25 +59,34 @@
         "--kuttl_test",
         help="Kuttl test suite definition file.",
         type=str,
         required=False,
         default="tests/kuttl-test.yaml.jinja2",
     )
 
+    parser.add_argument(
+        "-s",
+        "--suite",
+        help="Name of the test suite to expand. Default: default",
+        type=str,
+        required=False,
+        default="default",
+    )
+
     return parser.parse_args()
 
 
 def _cli_log_level(cli_arg: str) -> int:
     if cli_arg == "debug":
         return logging.DEBUG
     return logging.INFO
 
 
 def main() -> int:
     """Main"""
     cli_args = parse_cli_args()
     logging.basicConfig(
         encoding="utf-8", level=_cli_log_level(cli_args.log_level))
-    test_suite = TestSuite(cli_args.test_definition)
+    effective_test_suites = renderer_from_file(cli_args.test_definition)
     # Compatibility warning: add 'tests' to output_dir
     output_dir = path.join(cli_args.output_dir, "tests")
-    return test_suite.expand(cli_args.template_dir, output_dir, cli_args.kuttl_test)
+    return expand(cli_args.suite, effective_test_suites, cli_args.template_dir, output_dir, cli_args.kuttl_test)
```

## beku/testsuite.py

```diff
@@ -1,8 +1,8 @@
-"""Expand kuttl tests from templates."""
+"""Expand kuttl test from templates."""
 import logging
 import os
 import re
 from dataclasses import dataclass, field
 from functools import cached_property
 from itertools import product, chain
 from os import walk, path, makedirs
@@ -105,15 +105,15 @@
 @dataclass(frozen=True)
 class TestDefinition:
     """Test case definition."""
     name: str
     dimensions: List[str]
 
 
-TTestSuite = TypeVar(    # pylint: disable=invalid-name
+TTestSuite = TypeVar(  # pylint: disable=invalid-name
     "TTestSuite", bound="TestSuite")
 
 
 @dataclass(frozen=True)
 class TestSuite:
     """Test suite template."""
     source: str = field()
@@ -122,15 +122,15 @@
     def __post_init__(self) -> None:
         with open(self.source, encoding="utf8") as stream:
             tin = safe_load(stream)
             dimensions = [
                 TestDimension(d["name"], d["values"]) for d in tin["dimensions"]
             ]
             test_def = [
-                TestDefinition(t["name"], t["dimensions"]) for t in tin["tests"]
+                TestDefinition(t["name"], t["dimensions"]) for t in tin["test"]
             ]
             self.test_cases.extend(self._build(dimensions, test_def))
 
     @classmethod
     def _build(
             cls: Type[TTestSuite], dims: List[TestDimension], tests: List[TestDefinition]
     ) -> List[TestCase]:
@@ -174,20 +174,20 @@
                 f"Kuttl test config template not found [{kuttl_tests}]")
 
     def _expand_kuttl_tests(self, output_dir: str, kuttl_tests: str) -> None:
         env = Environment(loader=FileSystemLoader(path.dirname(kuttl_tests)))
         kt_base_name = path.basename(kuttl_tests)
         template = env.get_template(kt_base_name)
         kt_dest_name = re.sub(r"\.j(inja)?2$", "", kt_base_name)
-        # Compatibility warning: Assume output_dir ends with 'tests' and remove
+        # Compatibility warning: Assume output_dir ends with 'test' and remove
         # it from the destination file
         dest = path.join(path.dirname(output_dir), kt_dest_name)
         kuttl_vars = {
             "testinput": {
-                "tests": [{"name": tn} for tn in {tc.name for tc in self.test_cases}]
+                "test": [{"name": tn} for tn in {tc.name for tc in self.test_cases}]
             }
         }
         logging.debug("kuttl vars %s", kuttl_vars)
         with open(dest, encoding="utf8", mode="w") as stream:
             print(template.render(kuttl_vars), file=stream)
```

## beku/version.py

```diff
@@ -1,3 +1,3 @@
 """Package version."""
-__version_info__ = (0, 0, '6')
+__version_info__ = (0, 0, '7')
 __version__ = ".".join(map(str, __version_info__))
```

## tests/testsuite.py

```diff
@@ -1,12 +1,12 @@
 import textwrap
 import unittest
 from pprint import pprint
 
-from beku.testsuite import renderer_from_stream
+from beku.kuttl import renderer_from_stream
 
 
 class TestSum(unittest.TestCase):
     def test_load(self):
         fixture = textwrap.dedent("""
             ---
             dimensions:
@@ -21,15 +21,15 @@
               - name: zookeeper
                 values:
                   - 3.7.0-stackable0.0.0-dev
                   - 3.8.0-stackable0.0.0-dev
               - name: zookeeper-latest
                 values:
                   - 3.8.0-stackable0.0.0-dev
-            tests:
+            test:
               - name: smoke
                 dimensions:
                   - druid
                   - zookeeper
               - name: resources
                 dimensions:
                   - druid-latest
```

## Comparing `beku_stackabletech-0.0.6.dist-info/LICENSE` & `beku_stackabletech-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beku_stackabletech-0.0.6.dist-info/METADATA` & `beku_stackabletech-0.0.7.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: beku-stackabletech
-Version: 0.0.6
+Version: 0.0.7
 Summary: Test suite expander for Stackable Kuttl tests.
 Author-email: Razvan Mihai <razvan.mihai@stackable.tech>
 Project-URL: Homepage, https://github.com/stackabletech/beku.py
 Project-URL: Bug Tracker, https://github.com/stackabletech/beku.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jinja2 (>=3.1.2)
 Requires-Dist: PyYAML (>=6.0)
-Provides-Extra: dev
-Requires-Dist: pre-commit ; extra == 'dev'
 Provides-Extra: lint
-Requires-Dist: pylint ; extra == 'lint'
-Requires-Dist: mypy ; extra == 'lint'
+Requires-Dist: ruff (==0.0.275) ; extra == 'lint'
+Requires-Dist: mypy (==1.4.0) ; extra == 'lint'
 
 # beku
 
-Version: 0.0.6
+Version: 0.0.7
 
 ## Installation
 
-    pip install git+https://github.com/stackabletech/beku.py.git@0.0.6
+    pip install git+https://github.com/stackabletech/beku.py.git@master
 
 ## Usage
 
     cd <stackable operator directory>
     rm -rf tests/_work && beku
     cd tests/_work && kubectl kuttl test
 
+Also see the `examples` folder.
+
 ## Description
 
 Fast Kuttl tests expander for Stackable integration tests.
 
     beku -i tests/test-definition.yaml -t tests/templates/kuttl -k tests/kuttl-test.yaml.jinja2 -o tests/_work
 
 ## Release a new version
 
 Update the version in:
 
-* `pyptoject.toml`
+* `pyproject.toml`
 * `version.py`
 * `README.md`
 
 Update the CHANGELOG.
 Commit and tag.
 Build and publish:
+
     rm -rf dist/
     python -m build --wheel .
     twine upload dist/*
```

