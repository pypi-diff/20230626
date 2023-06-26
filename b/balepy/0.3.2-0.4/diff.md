# Comparing `tmp/balepy-0.3.2.tar.gz` & `tmp/balepy-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-0.3.2.tar", last modified: Mon Jun 26 18:23:56 2023, max compression
+gzip compressed data, was "balepy-0.4.tar", last modified: Mon Jun 26 18:29:51 2023, max compression
```

## Comparing `balepy-0.3.2.tar` & `balepy-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:23:56.010828 balepy-0.3.2/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.3.2/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-26 18:23:56.010828 balepy-0.3.2/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.3.2/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:23:56.007495 balepy-0.3.2/balepy/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1481 2023-06-26 18:23:07.000000 balepy-0.3.2/balepy/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:23:56.010828 balepy-0.3.2/balepy.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-26 18:23:56.010828 balepy-0.3.2/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      989 2023-06-26 18:23:38.000000 balepy-0.3.2/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:29:51.482501 balepy-0.4/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.4/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      990 2023-06-26 18:29:51.482501 balepy-0.4/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.4/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:29:51.482501 balepy-0.4/balepy/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1474 2023-06-26 18:28:33.000000 balepy-0.4/balepy/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:29:51.482501 balepy-0.4/balepy.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      990 2023-06-26 18:29:51.000000 balepy-0.4/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-06-26 18:29:51.000000 balepy-0.4/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-26 18:29:51.000000 balepy-0.4/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-06-26 18:29:51.000000 balepy-0.4/balepy.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-26 18:29:51.482501 balepy-0.4/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      987 2023-06-26 18:29:12.000000 balepy-0.4/setup.py
```

### Comparing `balepy-0.3.2/LICENSE` & `balepy-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `balepy-0.3.2/PKG-INFO` & `balepy-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.3.2
+Version: 0.4
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balepy-0.3.2/balepy/__init__.py` & `balepy-0.4/balepy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from requests import *
+import requests
 from colorama import Fore
 
 
 print(f"""Wellcom to{Fore.MAGENTA} balepy {Fore.RESET} library version:{Fore.LIGHTBLUE_EX} 0.1 {Fore.RESET}
 {Fore.GREEN}Mohammad Mehrabi Rad{Fore.RESET} and {Fore.RED}Erfan Bafandeh{Fore.RESET}{Fore.LIGHTMAGENTA_EX} <github.com/OnlyRad>{Fore.RESET}""")
 
 class Bot:
```

### Comparing `balepy-0.3.2/balepy.egg-info/PKG-INFO` & `balepy-0.4/balepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.3.2
+Version: 0.4
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balepy-0.3.2/setup.py` & `balepy-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '0.3.2',
+    version = '0.4',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bot API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

