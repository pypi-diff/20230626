# Comparing `tmp/iamlistening-0.2.1.tar.gz` & `tmp/iamlistening-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.2.1.tar", max compression
+gzip compressed data, was "iamlistening-0.2.2.tar", max compression
```

## Comparing `iamlistening-0.2.1.tar` & `iamlistening-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-25 20:15:30.373247 iamlistening-0.2.1/LICENSE
--rw-r--r--   0        0        0     1629 2023-06-25 20:15:30.373247 iamlistening-0.2.1/README.md
--rw-r--r--   0        0        0       99 2023-06-25 20:15:31.317301 iamlistening-0.2.1/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-06-25 20:15:30.373247 iamlistening-0.2.1/iamlistening/config.py
--rw-r--r--   0        0        0      868 2023-06-25 20:15:30.373247 iamlistening-0.2.1/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3839 2023-06-25 20:15:30.373247 iamlistening-0.2.1/iamlistening/main.py
--rw-r--r--   0        0        0     2163 2023-06-25 20:15:31.317301 iamlistening-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 iamlistening-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 21:12:44.170312 iamlistening-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1632 2023-06-25 21:12:44.170312 iamlistening-0.2.2/README.md
+-rw-r--r--   0        0        0       99 2023-06-25 21:12:45.102390 iamlistening-0.2.2/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-06-25 21:12:44.170312 iamlistening-0.2.2/iamlistening/config.py
+-rw-r--r--   0        0        0      868 2023-06-25 21:12:44.170312 iamlistening-0.2.2/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3839 2023-06-25 21:12:44.170312 iamlistening-0.2.2/iamlistening/main.py
+-rw-r--r--   0        0        0     2163 2023-06-25 21:12:45.098389 iamlistening-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 iamlistening-0.2.2/PKG-INFO
```

### Comparing `iamlistening-0.2.1/LICENSE` & `iamlistening-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.1/README.md` & `iamlistening-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # I Am Listening
 
 | <img width="200" alt="Logo" src="https://github.com/mraniki/iamlistening/assets/8766259/f76331f6-8821-49eb-8f1c-06aedd8557be"> | A python package to listen to messaging platforms. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN)](https://codecov.io/gh/mraniki/iamlistening) | build a client to interact with messaging platform|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%F0%9F%91%B7Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN)](https://codecov.io/gh/mraniki/iamlistening) | build a client to interact with messaging platform|
 
 Key features:
 
  - support discord, telegram and matrix platform
 
 ## Install
```

### Comparing `iamlistening-0.2.1/iamlistening/config.py` & `iamlistening-0.2.2/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.1/iamlistening/default_settings.toml` & `iamlistening-0.2.2/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.1/iamlistening/main.py` & `iamlistening-0.2.2/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.1/pyproject.toml` & `iamlistening-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.2.1"
+version = "0.2.2"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.2.1/PKG-INFO` & `iamlistening-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Project-URL: Support, https://github.com/mraniki/iamlistening/discussions
 Description-Content-Type: text/markdown
 
 # I Am Listening
 
 | <img width="200" alt="Logo" src="https://github.com/mraniki/iamlistening/assets/8766259/f76331f6-8821-49eb-8f1c-06aedd8557be"> | A python package to listen to messaging platforms. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN)](https://codecov.io/gh/mraniki/iamlistening) | build a client to interact with messaging platform|
+|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/iamlistening?icon=pypi&label)](https://pypi.org/project/iamlistening/) ![Version](https://img.shields.io/pypi/v/iamlistening)<br>  ![Pypi](https://img.shields.io/pypi/dm/iamlistening)<br> [![Build](https://github.com/mraniki/iamlistening/actions/workflows/%F0%9F%91%B7Flow.yml/badge.svg)](https://github.com/mraniki/listening/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN)](https://codecov.io/gh/mraniki/iamlistening) | build a client to interact with messaging platform|
 
 Key features:
 
  - support discord, telegram and matrix platform
 
 ## Install
```

