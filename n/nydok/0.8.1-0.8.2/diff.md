# Comparing `tmp/nydok-0.8.1.tar.gz` & `tmp/nydok-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nydok-0.8.1.tar", max compression
+gzip compressed data, was "nydok-0.8.2.tar", max compression
```

## Comparing `nydok-0.8.1.tar` & `nydok-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-06-06 13:48:15.366745 nydok-0.8.1/LICENSE
--rw-r--r--   0        0        0     3879 2023-06-06 13:48:15.366745 nydok-0.8.1/README.md
--rw-r--r--   0        0        0       52 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/__init__.py
--rw-r--r--   0        0        0     5444 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/cli.py
--rw-r--r--   0        0        0      227 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/exception.py
--rw-r--r--   0        0        0     4156 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/gitlab.py
--rw-r--r--   0        0        0       66 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/markdown_ext/__init__.py
--rw-r--r--   0        0        0     2174 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/markdown_ext/markdown_nydok.py
--rw-r--r--   0        0        0      572 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/markdown_ext/nydok.css
--rw-r--r--   0        0        0        0 2023-06-06 13:48:15.370745 nydok-0.8.1/nydok/plugin/__init__.py
--rw-r--r--   0        0        0     4001 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/plugin/junit.py
--rw-r--r--   0        0        0     4160 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/plugin/plugin.py
--rw-r--r--   0        0        0     3254 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/plugin/specification.py
--rw-r--r--   0        0        0     3240 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/plugin/specsmanager.py
--rw-r--r--   0        0        0     2226 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/plugin/testcase.py
--rw-r--r--   0        0        0    15037 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/report.py
--rw-r--r--   0        0        0     3805 2023-06-06 13:48:15.374745 nydok-0.8.1/nydok/schema.py
--rw-r--r--   0        0        0     1040 2023-06-06 13:50:20.428969 nydok-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 nydok-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 08:46:06.104549 nydok-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4270 2023-06-26 08:46:06.104549 nydok-0.8.2/README.md
+-rw-r--r--   0        0        0       52 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/__init__.py
+-rw-r--r--   0        0        0     5444 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/cli.py
+-rw-r--r--   0        0        0      227 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/exception.py
+-rw-r--r--   0        0        0     4156 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/gitlab.py
+-rw-r--r--   0        0        0       66 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/markdown_ext/__init__.py
+-rw-r--r--   0        0        0     2174 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/markdown_ext/markdown_nydok.py
+-rw-r--r--   0        0        0      572 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/markdown_ext/nydok.css
+-rw-r--r--   0        0        0        0 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/__init__.py
+-rw-r--r--   0        0        0     4001 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/junit.py
+-rw-r--r--   0        0        0     4157 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/plugin.py
+-rw-r--r--   0        0        0     3254 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/specification.py
+-rw-r--r--   0        0        0     3240 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/specsmanager.py
+-rw-r--r--   0        0        0     2226 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/testcase.py
+-rw-r--r--   0        0        0    15037 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/report.py
+-rw-r--r--   0        0        0     3805 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/schema.py
+-rw-r--r--   0        0        0     1040 2023-06-26 08:48:46.956481 nydok-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     5013 1970-01-01 00:00:00.000000 nydok-0.8.2/PKG-INFO
```

### Comparing `nydok-0.8.1/LICENSE` & `nydok-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/README.md` & `nydok-0.8.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <div align="center">
     <img src="https://github.com/nykodetherapeutics/nydok/raw/main/docs/assets/nydok-logo.png" width="70%">
 </div>
 
+[![Main](https://github.com/nykodetherapeutics/nydok/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/nykodetherapeutics/nydok/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/nydok.svg)](https://badge.fury.io/py/nydok)
+
+[Home page](https://nykodetherapeutics.github.io/nydok/) | [Getting started](https://nykodetherapeutics.github.io/nydok/intro/)
 
 **nydok** is a combined specification writing and testing framework, for producing consistent and traceable specification documents. It is developed for Computerized Systems Validation in a GAMP 5 / GxP context, but is applicable to any software development process where traceability is important.
 
 Write your requirements and risk assessment alongside your Python code, ensuring 1:1 mapping between requirements and the code you're writing.
 
 It is implemented as a plugin for `py.test` for running the tests, combined with a CLI for creating reports.
```

### Comparing `nydok-0.8.1/nydok/cli.py` & `nydok-0.8.2/nydok/cli.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/gitlab.py` & `nydok-0.8.2/nydok/gitlab.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/markdown_ext/markdown_nydok.py` & `nydok-0.8.2/nydok/markdown_ext/markdown_nydok.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/markdown_ext/nydok.css` & `nydok-0.8.2/nydok/markdown_ext/nydok.css`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/plugin/junit.py` & `nydok-0.8.2/nydok/plugin/junit.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/plugin/plugin.py` & `nydok-0.8.2/nydok/plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,18 +63,18 @@
     elif is_pytest_with_testcase(item):
         test_case = getattr(item.function, REQ_TESTCASE_TAG)
 
     if test_case:
         specs_manager.add_test_case(test_case)
 
     # Run the test
-    outcome = yield
+    result = yield
 
     # Update TestCase.passed if the test passed
-    if is_pytest_with_testcase(item) and not outcome._excinfo:
+    if is_pytest_with_testcase(item) and not result.excinfo:
         test_case.passed = True
 
 
 def pytest_collection_finish(session):
     """Runs after py.test is done collecting test Items.
 
     We need to ensure that all ReqItems runs last,
```

### Comparing `nydok-0.8.1/nydok/plugin/specification.py` & `nydok-0.8.2/nydok/plugin/specification.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/plugin/specsmanager.py` & `nydok-0.8.2/nydok/plugin/specsmanager.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/plugin/testcase.py` & `nydok-0.8.2/nydok/plugin/testcase.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/report.py` & `nydok-0.8.2/nydok/report.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/nydok/schema.py` & `nydok-0.8.2/nydok/schema.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.1/pyproject.toml` & `nydok-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nydok"
-version = "v0.8.1"
+version = "v0.8.2"
 description = "Documentation and specification testing framework"
 authors = ["Nykode Therapeutics <insaid@nykode.com>"]
 license = "MIT"
 classifiers = []
 packages = [
   { include = "nydok" }
 ]
```

### Comparing `nydok-0.8.1/PKG-INFO` & `nydok-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nydok
-Version: 0.8.1
+Version: 0.8.2
 Summary: Documentation and specification testing framework
 License: MIT
 Author: Nykode Therapeutics
 Author-email: insaid@nykode.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,17 @@
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://github.com/nykodetherapeutics/nydok/raw/main/docs/assets/nydok-logo.png" width="70%">
 </div>
 
+[![Main](https://github.com/nykodetherapeutics/nydok/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/nykodetherapeutics/nydok/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/nydok.svg)](https://badge.fury.io/py/nydok)
+
+[Home page](https://nykodetherapeutics.github.io/nydok/) | [Getting started](https://nykodetherapeutics.github.io/nydok/intro/)
 
 **nydok** is a combined specification writing and testing framework, for producing consistent and traceable specification documents. It is developed for Computerized Systems Validation in a GAMP 5 / GxP context, but is applicable to any software development process where traceability is important.
 
 Write your requirements and risk assessment alongside your Python code, ensuring 1:1 mapping between requirements and the code you're writing.
 
 It is implemented as a plugin for `py.test` for running the tests, combined with a CLI for creating reports.
```

