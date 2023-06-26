# Comparing `tmp/mareep-0.0.2.tar.gz` & `tmp/mareep-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mareep-0.0.2.tar", last modified: Sun Jun 25 13:11:55 2023, max compression
+gzip compressed data, was "mareep-0.0.3.tar", last modified: Mon Jun 26 02:14:09 2023, max compression
```

## Comparing `mareep-0.0.2.tar` & `mareep-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.911548 mareep-0.0.2/
--rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-25 13:11:55.911398 mareep-0.0.2/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.2/README.md
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.906562 mareep-0.0.2/mareep/
--rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.2/mareep/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.2/mareep/__main__.py
--rw-r--r--   0 datnh      (501) staff       (20)     2380 2023-06-25 08:08:40.000000 mareep-0.0.2/mareep/app.py
--rw-r--r--   0 datnh      (501) staff       (20)     1523 2023-06-25 10:04:13.000000 mareep-0.0.2/mareep/function.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.909714 mareep-0.0.2/mareep/loaders/
--rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.2/mareep/loaders/__init__.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.910326 mareep-0.0.2/mareep/loaders/json_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.2/mareep/loaders/json_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.2/mareep/loaders/json_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.2/mareep/loaders/loader.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.910974 mareep-0.0.2/mareep/loaders/yaml_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.2/mareep/loaders/yaml_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.2/mareep/loaders/yaml_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-06-25 13:06:37.000000 mareep-0.0.2/mareep/renderer.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-25 13:11:55.909227 mareep-0.0.2/mareep.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      494 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)       49 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/entry_points.txt
--rw-r--r--   0 datnh      (501) staff       (20)       55 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/requires.txt
--rw-r--r--   0 datnh      (501) staff       (20)        7 2023-06-25 13:11:55.000000 mareep-0.0.2/mareep.egg-info/top_level.txt
--rw-r--r--   0 datnh      (501) staff       (20)       38 2023-06-25 13:11:55.911595 mareep-0.0.2/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-06-25 13:05:28.000000 mareep-0.0.2/setup.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.145233 mareep-0.0.3/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-26 02:14:09.145091 mareep-0.0.3/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.3/README.md
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.142676 mareep-0.0.3/mareep/
+-rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.3/mareep/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.3/mareep/__main__.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2380 2023-06-25 08:08:40.000000 mareep-0.0.3/mareep/app.py
+-rw-r--r--   0 datnh      (501) staff       (20)     1557 2023-06-26 02:13:40.000000 mareep-0.0.3/mareep/function.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.143798 mareep-0.0.3/mareep/loaders/
+-rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.3/mareep/loaders/__init__.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.144409 mareep-0.0.3/mareep/loaders/json_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.3/mareep/loaders/json_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.3/mareep/loaders/json_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.3/mareep/loaders/loader.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.144777 mareep-0.0.3/mareep/loaders/yaml_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.3/mareep/loaders/yaml_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.3/mareep/loaders/yaml_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-06-25 13:06:37.000000 mareep-0.0.3/mareep/renderer.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.143539 mareep-0.0.3/mareep.egg-info/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      494 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/SOURCES.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        1 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/dependency_links.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       49 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/entry_points.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       55 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/requires.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        7 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/top_level.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       38 2023-06-26 02:14:09.145278 mareep-0.0.3/setup.cfg
+-rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-06-26 02:13:46.000000 mareep-0.0.3/setup.py
```

### Comparing `mareep-0.0.2/PKG-INFO` & `mareep-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mareep
-Version: 0.0.2
+Version: 0.0.3
 Summary: mareep
 Home-page: https://github.com/NgHoangDat/mareep.git
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mareep-0.0.2/mareep/app.py` & `mareep-0.0.3/mareep/app.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.2/mareep/function.py` & `mareep-0.0.3/mareep/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typer import Argument, Option, Context
 
 from .app import app
 from .renderer import Renderer
 
 
 @app.command(
-    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
+    context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
+    invoke_without_command=True,
 )
 def render(
     ctx: Context,
     template_path: Path = Argument(..., help="Template path"),
     output_path: Path = Argument(..., help="Output path"),
 
     extensions: List[str] = Option(["j2", "jinja2", "jinja"], help="List of templete extensions"),
```

### Comparing `mareep-0.0.2/mareep/loaders/__init__.py` & `mareep-0.0.3/mareep/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.2/mareep/renderer.py` & `mareep-0.0.3/mareep/renderer.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.2/mareep.egg-info/PKG-INFO` & `mareep-0.0.3/mareep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mareep
-Version: 0.0.2
+Version: 0.0.3
 Summary: mareep
 Home-page: https://github.com/NgHoangDat/mareep.git
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mareep-0.0.2/setup.py` & `mareep-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import *
 
 import setuptools
 
 __PACKAGE__ = "mareep"
-__VERSION__ = "0.0.2"
+__VERSION__ = "0.0.3"
 
 base_dir = Path(__file__).resolve().parent
 
 with open(base_dir / "README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

