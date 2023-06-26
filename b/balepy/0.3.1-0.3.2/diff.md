# Comparing `tmp/balepy-0.3.1.tar.gz` & `tmp/balepy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-0.3.1.tar", last modified: Mon Jun 26 18:15:11 2023, max compression
+gzip compressed data, was "balepy-0.3.2.tar", last modified: Mon Jun 26 18:23:56 2023, max compression
```

## Comparing `balepy-0.3.1.tar` & `balepy-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:15:11.880982 balepy-0.3.1/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.3.1/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-26 18:15:11.880982 balepy-0.3.1/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.3.1/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:15:11.880982 balepy-0.3.1/bale/
--rw-r--r--   0 themamad  (1000) themamad  (1000)       31 2023-06-26 18:13:59.000000 balepy-0.3.1/bale/__init__.py
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1485 2023-06-26 18:13:53.000000 balepy-0.3.1/bale/main.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:15:11.880982 balepy-0.3.1/balepy.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-26 18:15:11.000000 balepy-0.3.1/balepy.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      176 2023-06-26 18:15:11.000000 balepy-0.3.1/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-26 18:15:11.000000 balepy-0.3.1/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        5 2023-06-26 18:15:11.000000 balepy-0.3.1/balepy.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-26 18:15:11.880982 balepy-0.3.1/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      989 2023-06-26 18:14:50.000000 balepy-0.3.1/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:23:56.010828 balepy-0.3.2/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.3.2/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-26 18:23:56.010828 balepy-0.3.2/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.3.2/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:23:56.007495 balepy-0.3.2/balepy/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1481 2023-06-26 18:23:07.000000 balepy-0.3.2/balepy/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-26 18:23:56.010828 balepy-0.3.2/balepy.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      992 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-06-26 18:23:56.000000 balepy-0.3.2/balepy.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-26 18:23:56.010828 balepy-0.3.2/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      989 2023-06-26 18:23:38.000000 balepy-0.3.2/setup.py
```

### Comparing `balepy-0.3.1/LICENSE` & `balepy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `balepy-0.3.1/PKG-INFO` & `balepy-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.3.1
+Version: 0.3.2
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balepy-0.3.1/bale/main.py` & `balepy-0.3.2/balepy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from requests import *
 from colorama import Fore
 
 
 print(f"""Wellcom to{Fore.MAGENTA} balepy {Fore.RESET} library version:{Fore.LIGHTBLUE_EX} 0.1 {Fore.RESET}
 {Fore.GREEN}Mohammad Mehrabi Rad{Fore.RESET} and {Fore.RED}Erfan Bafandeh{Fore.RESET}{Fore.LIGHTMAGENTA_EX} <github.com/OnlyRad>{Fore.RESET}""")
 
-class methods:
+class Bot:
 
     def __init__(self , token:str):
         self.token = token
     
 
     def send_Message(self , chat_id:int , text:str):
         self.chat_id = chat_id
```

### Comparing `balepy-0.3.1/balepy.egg-info/PKG-INFO` & `balepy-0.3.2/balepy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.3.1
+Version: 0.3.2
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `balepy-0.3.1/setup.py` & `balepy-0.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '0.3.1',
+    version = '0.3.2',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bot API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

