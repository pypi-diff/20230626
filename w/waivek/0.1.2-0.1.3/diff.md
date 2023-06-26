# Comparing `tmp/waivek-0.1.2.tar.gz` & `tmp/waivek-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waivek-0.1.2.tar", last modified: Mon Jun 26 13:02:53 2023, max compression
+gzip compressed data, was "waivek-0.1.3.tar", last modified: Mon Jun 26 17:01:35 2023, max compression
```

## Comparing `waivek-0.1.2.tar` & `waivek-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 13:02:53.878125 waivek-0.1.2/
--rw-rw-rw-   0        0        0      141 2023-06-26 13:02:53.878125 waivek-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-26 13:02:53.878125 waivek-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-26 13:02:38.000000 waivek-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:02:53.851037 waivek-0.1.2/waivek/
--rw-rw-rw-   0        0        0      377 2023-06-26 13:02:23.000000 waivek-0.1.2/waivek/__init__.py
--rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.2/waivek/color.py
--rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.2/waivek/common.py
--rw-rw-rw-   0        0        0    18804 2023-06-26 13:00:50.000000 waivek-0.1.2/waivek/db.py
--rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.2/waivek/error.py
--rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.2/waivek/frame.py
--rw-rw-rw-   0        0        0     9044 2023-06-26 13:01:10.000000 waivek-0.1.2/waivek/get.py
--rw-rw-rw-   0        0        0    28068 2023-06-26 13:01:20.000000 waivek-0.1.2/waivek/ic.py
--rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.2/waivek/print_utils.py
--rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1.2/waivek/reltools.py
--rw-rw-rw-   0        0        0     4117 2023-06-26 13:01:32.000000 waivek-0.1.2/waivek/reqs.py
--rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.2/waivek/tdd.py
--rw-rw-rw-   0        0        0      395 2023-06-26 13:01:40.000000 waivek-0.1.2/waivek/template.py
--rw-rw-rw-   0        0        0    21659 2023-06-26 13:01:55.000000 waivek-0.1.2/waivek/test.py
--rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.2/waivek/timer.py
--rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.2/waivek/trace.py
-drwxrwxrwx   0        0        0        0 2023-06-26 13:02:53.878125 waivek-0.1.2/waivek.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-26 13:02:53.000000 waivek-0.1.2/waivek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-06-26 13:02:53.000000 waivek-0.1.2/waivek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 13:02:53.000000 waivek-0.1.2/waivek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-26 13:02:53.000000 waivek-0.1.2/waivek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       75 2023-06-26 13:02:53.000000 waivek-0.1.2/waivek.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 17:01:35.235937 waivek-0.1.3/
+-rw-rw-rw-   0        0        0      141 2023-06-26 17:01:35.235937 waivek-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:01:35.235937 waivek-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2023-06-26 17:01:23.000000 waivek-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:01:35.204686 waivek-0.1.3/waivek/
+-rw-rw-rw-   0        0        0      377 2023-06-26 13:32:15.000000 waivek-0.1.3/waivek/__init__.py
+-rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.3/waivek/color.py
+-rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.3/waivek/common.py
+-rw-rw-rw-   0        0        0    18804 2023-06-26 13:00:50.000000 waivek-0.1.3/waivek/db.py
+-rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.3/waivek/error.py
+-rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.3/waivek/frame.py
+-rw-rw-rw-   0        0        0     9044 2023-06-26 13:01:10.000000 waivek-0.1.3/waivek/get.py
+-rw-rw-rw-   0        0        0    28068 2023-06-26 13:01:20.000000 waivek-0.1.3/waivek/ic.py
+-rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.3/waivek/print_utils.py
+-rw-rw-rw-   0        0        0     1883 2022-09-26 11:19:33.000000 waivek-0.1.3/waivek/reltools.py
+-rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.3/waivek/reqs.py
+-rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.3/waivek/tdd.py
+-rw-rw-rw-   0        0        0      395 2023-06-26 13:01:40.000000 waivek-0.1.3/waivek/template.py
+-rw-rw-rw-   0        0        0    21659 2023-06-26 13:01:55.000000 waivek-0.1.3/waivek/test.py
+-rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.3/waivek/timer.py
+-rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.3/waivek/trace.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:01:35.235937 waivek-0.1.3/waivek.egg-info/
+-rw-rw-rw-   0        0        0      141 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 17:01:35.000000 waivek-0.1.3/waivek.egg-info/top_level.txt
```

### Comparing `waivek-0.1.2/waivek/color.py` & `waivek-0.1.3/waivek/color.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/common.py` & `waivek-0.1.3/waivek/common.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/db.py` & `waivek-0.1.3/waivek/db.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/error.py` & `waivek-0.1.3/waivek/error.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/frame.py` & `waivek-0.1.3/waivek/frame.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/get.py` & `waivek-0.1.3/waivek/get.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/ic.py` & `waivek-0.1.3/waivek/ic.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/print_utils.py` & `waivek-0.1.3/waivek/print_utils.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/reltools.py` & `waivek-0.1.3/waivek/reltools.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/reqs.py` & `waivek-0.1.3/waivek/reqs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-import sys; sys.path = [ "C:/users/vivek/Documents/Python/" ] + sys.path
+# import sys; sys.path = [ "C:/users/vivek/Documents/Python/" ] + sys.path
 from .timer import Timer   # Single Use
 timer = Timer()
 from .color import Code    # Multi-Use
 from .error import handler # Single Use
 from .ic import ic, ib     # Multi-Use, import time: 70ms - 110ms
 Code; ic; ib; handler
 from .reltools import rel2abs
 
 def main():
-    print_python_modules()
-    print()
-    # ic(get_untracked_python_files())
-    # ic(get_python_files())
-    # ic(get_non_python_files())
-    print_pipreqs()
+    # print_python_modules()
+    # print()
+    # print_pipreqs()
+    pypi_version()
+
+def pypi_version():
+    from .ic import ic
+    import requests
+    package_name = "waivek"
+    url = f"https://pypi.org/pypi/{package_name}/json"
+    resp = requests.get(url)
+    D = resp.json()
+    version = D["info"]["version"]
+    major, minor, patch = version.split(".")
+    patch = int(patch) + 1
+    new_version = f"V- {major}.{minor}.{patch}"
+    ic(new_version)
+    
 
 
 def print_python_modules():
     import os.path
     to_module_name = lambda path: os.path.splitext(os.path.basename(path))[0]
     helper_modules = [ 'frame.py', 'trace.py' ]
     ignore_modules = [ 'reqs.py', 'setup.py', 'tdd.py', 'template.py', 'test.py' ]
```

### Comparing `waivek-0.1.2/waivek/tdd.py` & `waivek-0.1.3/waivek/tdd.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/test.py` & `waivek-0.1.3/waivek/test.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/timer.py` & `waivek-0.1.3/waivek/timer.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.2/waivek/trace.py` & `waivek-0.1.3/waivek/trace.py`

 * *Files identical despite different names*

