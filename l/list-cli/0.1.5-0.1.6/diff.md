# Comparing `tmp/list-cli-0.1.5.tar.gz` & `tmp/list-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list-cli-0.1.5.tar", last modified: Sun May 28 19:18:01 2023, max compression
+gzip compressed data, was "list-cli-0.1.6.tar", last modified: Mon Jun 26 10:33:22 2023, max compression
```

## Comparing `list-cli-0.1.5.tar` & `list-cli-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-28 19:18:01.121319 list-cli-0.1.5/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.5/LICENSE
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-28 19:18:01.121388 list-cli-0.1.5/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.5/README.md
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-28 19:18:01.120357 list-cli-0.1.5/list_cli/
--rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.5/list_cli/__init__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)     1659 2023-05-17 03:52:05.000000 list-cli-0.1.5/list_cli/__main__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-28 19:17:06.000000 list-cli-0.1.5/list_cli/__version__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)    12511 2023-05-28 19:13:53.000000 list-cli-0.1.5/list_cli/processors.py
--rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.5/list_cli/results.py
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-28 19:18:01.121205 list-cli-0.1.5/list_cli.egg-info/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/entry_points.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-28 19:18:01.000000 list-cli-0.1.5/list_cli.egg-info/top_level.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-28 19:18:01.121586 list-cli-0.1.5/setup.cfg
--rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.5/setup.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-06-26 10:33:22.164819 list-cli-0.1.6/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.6/LICENSE
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-06-26 10:33:22.164892 list-cli-0.1.6/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.6/README.md
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-06-26 10:33:22.163855 list-cli-0.1.6/list_cli/
+-rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.6/list_cli/__init__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1677 2023-06-26 10:33:15.000000 list-cli-0.1.6/list_cli/__main__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-06-26 10:33:15.000000 list-cli-0.1.6/list_cli/__version__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)    12511 2023-05-28 19:13:53.000000 list-cli-0.1.6/list_cli/processors.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.6/list_cli/results.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-06-26 10:33:22.164684 list-cli-0.1.6/list_cli.egg-info/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-06-26 10:33:22.000000 list-cli-0.1.6/list_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-06-26 10:33:22.000000 list-cli-0.1.6/list_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-06-26 10:33:22.000000 list-cli-0.1.6/list_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-06-26 10:33:22.000000 list-cli-0.1.6/list_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-06-26 10:33:22.000000 list-cli-0.1.6/list_cli.egg-info/top_level.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-06-26 10:33:22.165110 list-cli-0.1.6/setup.cfg
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.6/setup.py
```

### Comparing `list-cli-0.1.5/LICENSE` & `list-cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.5/PKG-INFO` & `list-cli-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.5/README.md` & `list-cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.5/list_cli/__main__.py` & `list-cli-0.1.6/list_cli/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,19 @@
     getcwd,
     getenv
 )
 from os.path import isfile, join as path_join
 from sys import argv, exit
 from typing import List
 
-from list_cli.processors import MultiProcessor, Processor
+from list_cli.processors import (
+    BaseProcessor,
+    MultiProcessor,
+    Processor
+)
 
 
 def _env_list_value(key, default='') -> List[str]:
     return list(filter(None, getenv(key, default).split(',')))
 
 
 def _get_database_file_paths() -> List[str]:
@@ -35,15 +39,15 @@
                 '.list',
                 database_name
             )
         )
     return database_file_paths
 
 
-def _get_processor(database_file_paths: List[str]) -> MultiProcessor | Processor:
+def _get_processor(database_file_paths: List[str]) -> BaseProcessor:
     if len(database_file_paths) > 1:
         return MultiProcessor(database_file_paths)
     return Processor(database_file_paths[0])
 
 
 def main():
     database_file_paths = _get_database_file_paths()
```

### Comparing `list-cli-0.1.5/list_cli/processors.py` & `list-cli-0.1.6/list_cli/processors.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.5/list_cli/results.py` & `list-cli-0.1.6/list_cli/results.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.5/list_cli.egg-info/PKG-INFO` & `list-cli-0.1.6/list_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.5/setup.py` & `list-cli-0.1.6/setup.py`

 * *Files identical despite different names*

