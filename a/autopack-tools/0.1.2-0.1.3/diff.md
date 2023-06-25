# Comparing `tmp/autopack_tools-0.1.2.tar.gz` & `tmp/autopack_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.1.2.tar", max compression
+gzip compressed data, was "autopack_tools-0.1.3.tar", max compression
```

## Comparing `autopack_tools-0.1.2.tar` & `autopack_tools-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     2920 2023-06-25 23:13:00.716562 autopack_tools-0.1.2/README.md
--rw-r--r--   0        0        0        6 2023-06-23 17:23:28.293631 autopack_tools-0.1.2/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-23 17:23:28.293676 autopack_tools-0.1.2/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-23 17:23:28.293853 autopack_tools-0.1.2/autopack/__main__.py
--rw-r--r--   0        0        0     1427 2023-06-25 23:11:09.434943 autopack_tools-0.1.2/autopack/api.py
--rw-r--r--   0        0        0      864 2023-06-23 17:24:04.323693 autopack_tools-0.1.2/autopack/cli.py
--rw-r--r--   0        0        0      258 2023-06-23 17:23:28.294559 autopack_tools-0.1.2/autopack/errors.py
--rw-r--r--   0        0        0     4459 2023-06-25 22:40:48.296677 autopack_tools-0.1.2/autopack/get_pack.py
--rw-r--r--   0        0        0     2679 2023-06-23 17:24:04.352595 autopack_tools-0.1.2/autopack/installation.py
--rw-r--r--   0        0        0      796 2023-06-25 23:15:45.962407 autopack_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3481 1970-01-01 00:00:00.000000 autopack_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2920 2023-06-25 23:21:07.938300 autopack_tools-0.1.3/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.3/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.3/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.3/autopack/__main__.py
+-rw-r--r--   0        0        0     1427 2023-06-25 23:21:07.938595 autopack_tools-0.1.3/autopack/api.py
+-rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.3/autopack/cli.py
+-rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.3/autopack/errors.py
+-rw-r--r--   0        0        0     4459 2023-06-25 23:21:01.957572 autopack_tools-0.1.3/autopack/get_pack.py
+-rw-r--r--   0        0        0     2679 2023-06-25 23:21:01.957868 autopack_tools-0.1.3/autopack/installation.py
+-rw-r--r--   0        0        0      883 2023-06-25 23:23:14.408748 autopack_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3576 1970-01-01 00:00:00.000000 autopack_tools-0.1.3/PKG-INFO
```

### Comparing `autopack_tools-0.1.2/README.md` & `autopack_tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.2/autopack/api.py` & `autopack_tools-0.1.3/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.2/autopack/cli.py` & `autopack_tools-0.1.3/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.2/autopack/get_pack.py` & `autopack_tools-0.1.3/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.2/autopack/installation.py` & `autopack_tools-0.1.3/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.2/pyproject.toml` & `autopack_tools-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.1.2"
+version = "0.1.3"
+repository = "https://github.com/AutoPackAI/autopack"
+homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
 
 [tool.poetry.scripts]
```

### Comparing `autopack_tools-0.1.2/PKG-INFO` & `autopack_tools-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package Manager for AI Agent tools
+Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
+Project-URL: Repository, https://github.com/AutoPackAI/autopack
 Description-Content-Type: text/markdown
 
 # AutoPack Tools
 
 [AutoPack](https://autopack.ai) is a repository for tools that are specifically designed for AI Agents.
 
 The `autopack-tools` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
```

