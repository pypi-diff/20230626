# Comparing `tmp/talkytrend-1.5.1.tar.gz` & `tmp/talkytrend-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.1.tar", max compression
+gzip compressed data, was "talkytrend-1.5.2.tar", max compression
```

## Comparing `talkytrend-1.5.1.tar` & `talkytrend-1.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-25 20:15:47.768488 talkytrend-1.5.1/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-25 20:15:47.768488 talkytrend-1.5.1/README.md
--rw-r--r--   0        0        0     2178 2023-06-25 20:15:48.480488 talkytrend-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-25 20:15:48.480488 talkytrend-1.5.1/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-25 20:15:47.768488 talkytrend-1.5.1/talkytrend/config.py
--rw-r--r--   0        0        0     1653 2023-06-25 20:15:47.768488 talkytrend-1.5.1/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6419 2023-06-25 20:15:47.768488 talkytrend-1.5.1/talkytrend/main.py
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 talkytrend-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-26 14:27:59.521110 talkytrend-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2190 2023-06-26 14:27:59.521110 talkytrend-1.5.2/README.md
+-rw-r--r--   0        0        0     2178 2023-06-26 14:28:00.329120 talkytrend-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-26 14:28:00.329120 talkytrend-1.5.2/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-26 14:27:59.521110 talkytrend-1.5.2/talkytrend/config.py
+-rw-r--r--   0        0        0     1653 2023-06-26 14:27:59.521110 talkytrend-1.5.2/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6419 2023-06-26 14:27:59.521110 talkytrend-1.5.2/talkytrend/main.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.2/PKG-INFO
```

### Comparing `talkytrend-1.5.1/LICENSE` & `talkytrend-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.1/README.md` & `talkytrend-1.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # TalkyTrend 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"> | A python package to retrieve asset trend and economic data. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) ![Version](https://img.shields.io/pypi/v/talkytrend)<br>  ![Pypi](https://img.shields.io/pypi/dm/talkytrend)<br> [![Build](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) | Find Asset Trend |
+|<br> 
+[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) [![Version](https://img.shields.io/pypi/v/talkytrend)]()<br> [![Pypi](https://img.shields.io/pypi/dm/talkytrend)]()<br> [![👷‍♂️Build](https://github.com/mraniki/talkytrend/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)]() <br>[![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) [![codebeat badge](https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6)](https://codebeat.co/projects/github-com-mraniki-talkytrend-main) | Find Asset Trend |
 
 Key features:
 
 - trading view connectivity
 
 ## Install
```

### Comparing `talkytrend-1.5.1/pyproject.toml` & `talkytrend-1.5.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.1"
+version = "1.5.2"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.1/talkytrend/config.py` & `talkytrend-1.5.2/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.1/talkytrend/default_settings.toml` & `talkytrend-1.5.2/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.1/talkytrend/main.py` & `talkytrend-1.5.2/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.1/PKG-INFO` & `talkytrend-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,16 @@
 Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 
 # TalkyTrend 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"> | A python package to retrieve asset trend and economic data. |
 | ------------- | ------------- |
-|<br> [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) ![Version](https://img.shields.io/pypi/v/talkytrend)<br>  ![Pypi](https://img.shields.io/pypi/dm/talkytrend)<br> [![Build](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/talkytrend/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) | Find Asset Trend |
+|<br> 
+[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) [![Version](https://img.shields.io/pypi/v/talkytrend)]()<br> [![Pypi](https://img.shields.io/pypi/dm/talkytrend)]()<br> [![👷‍♂️Build](https://github.com/mraniki/talkytrend/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)]() <br>[![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) [![codebeat badge](https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6)](https://codebeat.co/projects/github-com-mraniki-talkytrend-main) | Find Asset Trend |
 
 Key features:
 
 - trading view connectivity
 
 ## Install
```

