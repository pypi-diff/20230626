# Comparing `tmp/jupytercards-2.5.5.tar.gz` & `tmp/jupytercards-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jupytercards-2.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jupytercards-2.5.5.tar` & `jupytercards-2.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.5/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.5/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.5/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     4210 2023-05-17 20:46:04.470697 jupytercards-2.5.5/README.md
--rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.5/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.5/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.5/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.5/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-05-28 20:58:35.835257 jupytercards-2.5.5/jupytercards/__init__.py
--rw-r--r--   0        0        0     9737 2023-05-19 14:00:07.262578 jupytercards-2.5.5/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10291 2023-05-17 20:41:22.769979 jupytercards-2.5.5/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4235 2023-05-28 20:48:05.228974 jupytercards-2.5.5/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.5/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.5/pyproject.toml
--rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 jupytercards-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.6/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.6/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.6/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     4210 2023-05-17 20:46:04.470697 jupytercards-2.5.6/README.md
+-rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.6/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.6/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.6/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.6/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-06-26 13:39:02.780608 jupytercards-2.5.6/jupytercards/__init__.py
+-rw-r--r--   0        0        0     9732 2023-06-26 13:36:33.264198 jupytercards-2.5.6/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10291 2023-05-17 20:41:22.769979 jupytercards-2.5.6/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4235 2023-05-28 20:48:05.228974 jupytercards-2.5.6/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.6/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 jupytercards-2.5.6/PKG-INFO
```

### Comparing `jupytercards-2.5.5/.gitignore` & `jupytercards-2.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/LICENSE` & `jupytercards-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/Markdown-flashcards.ipynb` & `jupytercards-2.5.6/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/README.md` & `jupytercards-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/example.ipynb` & `jupytercards-2.5.6/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/extractdefinitions.py` & `jupytercards-2.5.6/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/flashcards.gif` & `jupytercards-2.5.6/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/jupytercards/__init__.py` & `jupytercards-2.5.6/jupytercards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.5.5'
+__version__ = '2.5.6'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.5.5/jupytercards/dynamic.py` & `jupytercards-2.5.6/jupytercards/dynamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-from IPython.core.display import display,  HTML, Javascript
+from IPython.display import display,  HTML, Javascript
 import string
 import random
 import json
 import urllib.request
 #import pkg_resources
 import importlib.resources
 import sys
```

### Comparing `jupytercards-2.5.5/jupytercards/flashcards.js` & `jupytercards-2.5.6/jupytercards/flashcards.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/jupytercards/styles.css` & `jupytercards-2.5.6/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/jupytercards/swiped-events.min.js` & `jupytercards-2.5.6/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.5/PKG-INFO` & `jupytercards-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.5.5
+Version: 2.5.6
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

