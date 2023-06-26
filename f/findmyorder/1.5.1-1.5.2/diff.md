# Comparing `tmp/findmyorder-1.5.1.tar.gz` & `tmp/findmyorder-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.1.tar", max compression
+gzip compressed data, was "findmyorder-1.5.2.tar", max compression
```

## Comparing `findmyorder-1.5.1.tar` & `findmyorder-1.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-25 20:15:21.306655 findmyorder-1.5.1/LICENSE
--rw-r--r--   0        0        0     1995 2023-06-25 20:15:21.306655 findmyorder-1.5.1/README.md
--rw-r--r--   0        0        0      113 2023-06-25 20:15:22.022675 findmyorder-1.5.1/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-06-25 20:15:21.306655 findmyorder-1.5.1/findmyorder/config.py
--rw-r--r--   0        0        0     2265 2023-06-25 20:15:21.306655 findmyorder-1.5.1/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5555 2023-06-25 20:15:21.306655 findmyorder-1.5.1/findmyorder/main.py
--rw-r--r--   0        0        0     2132 2023-06-25 20:15:22.022675 findmyorder-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 findmyorder-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-26 19:19:02.821749 findmyorder-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2219 2023-06-26 19:19:02.821749 findmyorder-1.5.2/README.md
+-rw-r--r--   0        0        0      113 2023-06-26 19:19:03.529761 findmyorder-1.5.2/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-06-26 19:19:02.821749 findmyorder-1.5.2/findmyorder/config.py
+-rw-r--r--   0        0        0     2265 2023-06-26 19:19:02.821749 findmyorder-1.5.2/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5555 2023-06-26 19:19:02.821749 findmyorder-1.5.2/findmyorder/main.py
+-rw-r--r--   0        0        0     2132 2023-06-26 19:19:03.529761 findmyorder-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 findmyorder-1.5.2/PKG-INFO
```

### Comparing `findmyorder-1.5.1/LICENSE` & `findmyorder-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.1/README.md` & `findmyorder-1.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: findmyorder
+Version: 1.5.2
+Summary: A python package to identify and parse order for trade execution.
+License: MIT
+Keywords: trading,order,trade,buy,sell
+Author: mraniki
+Author-email: 8766259+mraniki@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: emoji (>=2.5.1,<3.0.0)
+Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
+Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
+Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
+Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
+Description-Content-Type: text/markdown
+
 # Find my order
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![👷‍♂️Flow](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml)  [![codebeat badge](https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a)](https://codebeat.co/projects/github-com-mraniki-findmyorder-main) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
 
@@ -31,7 +52,8 @@
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 ## Documentation
 
 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
+
```

### Comparing `findmyorder-1.5.1/findmyorder/config.py` & `findmyorder-1.5.2/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.1/findmyorder/default_settings.toml` & `findmyorder-1.5.2/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.1/findmyorder/main.py` & `findmyorder-1.5.2/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.1/pyproject.toml` & `findmyorder-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.1"
+version = "1.5.2"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.5.1/PKG-INFO` & `findmyorder-1.5.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,12 @@
-Metadata-Version: 2.1
-Name: findmyorder
-Version: 1.5.1
-Summary: A python package to identify and parse order for trade execution.
-License: MIT
-Keywords: trading,order,trade,buy,sell
-Author: mraniki
-Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
-Requires-Dist: emoji (>=2.5.1,<3.0.0)
-Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
-Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
-Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
-Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
-Description-Content-Type: text/markdown
-
 # Find my order
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and <br>parse order for trade execution. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![👷‍♂️Flow](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml)  [![codebeat badge](https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a)](https://codebeat.co/projects/github-com-mraniki-findmyorder-main) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
 - Settings for custom option
 
@@ -52,8 +31,7 @@
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 ## Documentation
 
 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/)
-
```

