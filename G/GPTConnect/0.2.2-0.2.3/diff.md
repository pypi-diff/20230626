# Comparing `tmp/GPTConnect-0.2.2.tar.gz` & `tmp/GPTConnect-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.2.2.tar", last modified: Sun Jun 25 06:35:06 2023, max compression
+gzip compressed data, was "GPTConnect-0.2.3.tar", last modified: Mon Jun 26 05:07:06 2023, max compression
```

## Comparing `GPTConnect-0.2.2.tar` & `GPTConnect-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 06:35:06.716525 GPTConnect-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 06:35:06.704817 GPTConnect-0.2.2/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0     1222 2023-06-25 06:35:06.000000 GPTConnect-0.2.2/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-25 06:35:06.000000 GPTConnect-0.2.2/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 06:35:06.000000 GPTConnect-0.2.2/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-25 06:35:06.000000 GPTConnect-0.2.2/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-25 06:35:06.000000 GPTConnect-0.2.2/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2023-06-25 05:39:53.000000 GPTConnect-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1222 2023-06-25 06:35:06.715632 GPTConnect-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      992 2023-06-25 05:44:14.000000 GPTConnect-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 06:35:06.713630 GPTConnect-0.2.2/gptconnect/
--rw-rw-rw-   0        0        0       90 2023-06-24 09:26:23.000000 GPTConnect-0.2.2/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2830 2023-06-24 09:31:52.000000 GPTConnect-0.2.2/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.2.2/gptconnect/gptfunction.py
--rw-rw-rw-   0        0        0      382 2023-06-25 06:33:58.000000 GPTConnect-0.2.2/gptconnect/gptfunctionhandler.py
--rw-rw-rw-   0        0        0       42 2023-06-25 06:35:06.716525 GPTConnect-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-06-25 06:34:36.000000 GPTConnect-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 05:07:06.556788 GPTConnect-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-06-26 05:07:06.543753 GPTConnect-0.2.3/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-06-26 05:07:06.000000 GPTConnect-0.2.3/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-26 05:07:06.000000 GPTConnect-0.2.3/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 05:07:06.000000 GPTConnect-0.2.3/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 05:07:06.000000 GPTConnect-0.2.3/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 05:07:06.000000 GPTConnect-0.2.3/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-06-25 05:39:53.000000 GPTConnect-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1380 2023-06-26 05:07:06.555790 GPTConnect-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2023-06-26 05:06:39.000000 GPTConnect-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 05:07:06.553786 GPTConnect-0.2.3/gptconnect/
+-rw-rw-rw-   0        0        0      118 2023-06-26 04:19:52.000000 GPTConnect-0.2.3/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0      728 2023-06-26 05:05:04.000000 GPTConnect-0.2.3/gptconnect/dataclasses.py
+-rw-rw-rw-   0        0        0     2830 2023-06-26 04:57:37.000000 GPTConnect-0.2.3/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0     1005 2023-06-26 04:57:26.000000 GPTConnect-0.2.3/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0      382 2023-06-25 06:33:58.000000 GPTConnect-0.2.3/gptconnect/gptfunctionhandler.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 05:07:06.556788 GPTConnect-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-06-26 05:02:38.000000 GPTConnect-0.2.3/setup.py
```

### Comparing `GPTConnect-0.2.2/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.2.3/GPTConnect.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 License: Apache 2.0
 License-File: LICENSE
 
 # GPTConnect
 
+![PyPI - Downloads](https://img.shields.io/pypi/dd/gptconnect?color=success)
+![PyPI](https://img.shields.io/pypi/v/gptconnect?label=version&color=blue)
+
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
 
 Make sure to star this project if you find it useful! ✨
 
 If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
 ## 🔧 Features
@@ -22,8 +25,9 @@
 - 🕐 More features coming soon! This package is only in early stages of development.
 
 ## 🚀 Install
 `pip install GPTConnect`
 
 ## Example Usage
 [example-simple.py](https://github.com/SleepyStew/gptconnect/blob/master/example-simple.py)
+
 [example-advanced.py](https://github.com/SleepyStew/gptconnect/blob/master/example-advanced.py)
```

### Comparing `GPTConnect-0.2.2/LICENSE` & `GPTConnect-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.2.2/PKG-INFO` & `GPTConnect-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 License: Apache 2.0
 License-File: LICENSE
 
 # GPTConnect
 
+![PyPI - Downloads](https://img.shields.io/pypi/dd/gptconnect?color=success)
+![PyPI](https://img.shields.io/pypi/v/gptconnect?label=version&color=blue)
+
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
 
 Make sure to star this project if you find it useful! ✨
 
 If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
 ## 🔧 Features
@@ -22,8 +25,9 @@
 - 🕐 More features coming soon! This package is only in early stages of development.
 
 ## 🚀 Install
 `pip install GPTConnect`
 
 ## Example Usage
 [example-simple.py](https://github.com/SleepyStew/gptconnect/blob/master/example-simple.py)
+
 [example-advanced.py](https://github.com/SleepyStew/gptconnect/blob/master/example-advanced.py)
```

### Comparing `GPTConnect-0.2.2/README.md` & `GPTConnect-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # GPTConnect
 
+![PyPI - Downloads](https://img.shields.io/pypi/dd/gptconnect?color=success)
+![PyPI](https://img.shields.io/pypi/v/gptconnect?label=version&color=blue)
+
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
 
 Make sure to star this project if you find it useful! ✨
 
 If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
 ## 🔧 Features
@@ -13,8 +16,9 @@
 - 🕐 More features coming soon! This package is only in early stages of development.
 
 ## 🚀 Install
 `pip install GPTConnect`
 
 ## Example Usage
 [example-simple.py](https://github.com/SleepyStew/gptconnect/blob/master/example-simple.py)
+
 [example-advanced.py](https://github.com/SleepyStew/gptconnect/blob/master/example-advanced.py)
```

### Comparing `GPTConnect-0.2.2/gptconnect/gptconnect.py` & `GPTConnect-0.2.3/gptconnect/gptconnect.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import copy
 import json
 from typing import Union
-import openai
-import copy
 
+import openai
 
 valid_models = ["gpt-3.5-turbo-0613", "gpt-4-0613", "gpt-4-32k-0613"]
 functions = []
 
 
 class GPTConnect:
     """
```

