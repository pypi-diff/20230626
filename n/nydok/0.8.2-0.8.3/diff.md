# Comparing `tmp/nydok-0.8.2.tar.gz` & `tmp/nydok-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nydok-0.8.2.tar", max compression
+gzip compressed data, was "nydok-0.8.3.tar", max compression
```

## Comparing `nydok-0.8.2.tar` & `nydok-0.8.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-06-26 08:46:06.104549 nydok-0.8.2/LICENSE
--rw-r--r--   0        0        0     4270 2023-06-26 08:46:06.104549 nydok-0.8.2/README.md
--rw-r--r--   0        0        0       52 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/__init__.py
--rw-r--r--   0        0        0     5444 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/cli.py
--rw-r--r--   0        0        0      227 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/exception.py
--rw-r--r--   0        0        0     4156 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/gitlab.py
--rw-r--r--   0        0        0       66 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/markdown_ext/__init__.py
--rw-r--r--   0        0        0     2174 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/markdown_ext/markdown_nydok.py
--rw-r--r--   0        0        0      572 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/markdown_ext/nydok.css
--rw-r--r--   0        0        0        0 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/__init__.py
--rw-r--r--   0        0        0     4001 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/junit.py
--rw-r--r--   0        0        0     4157 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/plugin.py
--rw-r--r--   0        0        0     3254 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/specification.py
--rw-r--r--   0        0        0     3240 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/specsmanager.py
--rw-r--r--   0        0        0     2226 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/plugin/testcase.py
--rw-r--r--   0        0        0    15037 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/report.py
--rw-r--r--   0        0        0     3805 2023-06-26 08:46:06.112549 nydok-0.8.2/nydok/schema.py
--rw-r--r--   0        0        0     1040 2023-06-26 08:48:46.956481 nydok-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     5013 1970-01-01 00:00:00.000000 nydok-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 15:19:05.133282 nydok-0.8.3/LICENSE
+-rw-r--r--   0        0        0     4270 2023-06-26 15:19:05.133282 nydok-0.8.3/README.md
+-rw-r--r--   0        0        0       52 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/__init__.py
+-rw-r--r--   0        0        0     5444 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/cli.py
+-rw-r--r--   0        0        0      227 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/exception.py
+-rw-r--r--   0        0        0     4156 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/gitlab.py
+-rw-r--r--   0        0        0       66 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/markdown_ext/__init__.py
+-rw-r--r--   0        0        0     2174 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/markdown_ext/markdown_nydok.py
+-rw-r--r--   0        0        0      572 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/markdown_ext/nydok.css
+-rw-r--r--   0        0        0        0 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/plugin/__init__.py
+-rw-r--r--   0        0        0     4001 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/plugin/junit.py
+-rw-r--r--   0        0        0     4157 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/plugin/plugin.py
+-rw-r--r--   0        0        0     3254 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/plugin/specification.py
+-rw-r--r--   0        0        0     3240 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/plugin/specsmanager.py
+-rw-r--r--   0        0        0     2226 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/plugin/testcase.py
+-rw-r--r--   0        0        0    15037 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/report.py
+-rw-r--r--   0        0        0     3805 2023-06-26 15:19:05.141282 nydok-0.8.3/nydok/schema.py
+-rw-r--r--   0        0        0     1046 2023-06-26 15:21:05.430937 nydok-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     4980 1970-01-01 00:00:00.000000 nydok-0.8.3/PKG-INFO
```

### Comparing `nydok-0.8.2/LICENSE` & `nydok-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/README.md` & `nydok-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/cli.py` & `nydok-0.8.3/nydok/cli.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/gitlab.py` & `nydok-0.8.3/nydok/gitlab.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/markdown_ext/markdown_nydok.py` & `nydok-0.8.3/nydok/markdown_ext/markdown_nydok.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/markdown_ext/nydok.css` & `nydok-0.8.3/nydok/markdown_ext/nydok.css`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/plugin/junit.py` & `nydok-0.8.3/nydok/plugin/junit.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/plugin/plugin.py` & `nydok-0.8.3/nydok/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/plugin/specification.py` & `nydok-0.8.3/nydok/plugin/specification.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/plugin/specsmanager.py` & `nydok-0.8.3/nydok/plugin/specsmanager.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/plugin/testcase.py` & `nydok-0.8.3/nydok/plugin/testcase.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/report.py` & `nydok-0.8.3/nydok/report.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/nydok/schema.py` & `nydok-0.8.3/nydok/schema.py`

 * *Files identical despite different names*

### Comparing `nydok-0.8.2/pyproject.toml` & `nydok-0.8.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nydok"
-version = "v0.8.2"
+version = "v0.8.3"
 description = "Documentation and specification testing framework"
 authors = ["Nykode Therapeutics <insaid@nykode.com>"]
 license = "MIT"
 classifiers = []
 packages = [
   { include = "nydok" }
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pytest = "^6.2.3"
-PyYAML = "^6.0"
-requests = "^2.28.1"
-lxml = "^4.9.1"
-click = "^8.1.3"
+pytest = ">=6.2.5"
+PyYAML = ">=6.0"
+requests = ">=2.28.1"
+lxml = ">=4.8.0"
+click = ">=8.0.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^3.9.1"
 black = "^22.3.0"
 pytest-cov = "^2.11.1"
 coverage = {extras = ["toml"], version = "^5.5"}
 mypy = "^0.910"
@@ -46,8 +46,8 @@
 
 [tool.coverage.run]
 omit = [ "tests/*" ]
 
 [tool.isort]
 profile = "black"
 
-# For flake8, see .flake8
+# For flake8, see .flake8
```

### Comparing `nydok-0.8.2/PKG-INFO` & `nydok-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nydok
-Version: 0.8.2
+Version: 0.8.3
 Summary: Documentation and specification testing framework
 License: MIT
 Author: Nykode Therapeutics
 Author-email: insaid@nykode.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: pytest (>=6.2.3,<7.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: PyYAML (>=6.0)
+Requires-Dist: click (>=8.0.0)
+Requires-Dist: lxml (>=4.8.0)
+Requires-Dist: pytest (>=6.2.5)
+Requires-Dist: requests (>=2.28.1)
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://github.com/nykodetherapeutics/nydok/raw/main/docs/assets/nydok-logo.png" width="70%">
 </div>
 
 [![Main](https://github.com/nykodetherapeutics/nydok/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/nykodetherapeutics/nydok/actions/workflows/main.yml) [![PyPI version](https://badge.fury.io/py/nydok.svg)](https://badge.fury.io/py/nydok)
```

