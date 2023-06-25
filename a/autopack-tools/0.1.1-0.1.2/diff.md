# Comparing `tmp/autopack_tools-0.1.1.tar.gz` & `tmp/autopack_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.1.1.tar", max compression
+gzip compressed data, was "autopack_tools-0.1.2.tar", max compression
```

## Comparing `autopack_tools-0.1.1.tar` & `autopack_tools-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2896 2023-06-23 17:23:28.293501 autopack_tools-0.1.1/README.md
--rw-r--r--   0        0        0        6 2023-06-23 17:23:28.293631 autopack_tools-0.1.1/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-23 17:23:28.293676 autopack_tools-0.1.1/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-23 17:23:28.293853 autopack_tools-0.1.1/autopack/__main__.py
--rw-r--r--   0        0        0     1427 2023-06-25 23:11:09.434943 autopack_tools-0.1.1/autopack/api.py
--rw-r--r--   0        0        0      864 2023-06-23 17:24:04.323693 autopack_tools-0.1.1/autopack/cli.py
--rw-r--r--   0        0        0      258 2023-06-23 17:23:28.294559 autopack_tools-0.1.1/autopack/errors.py
--rw-r--r--   0        0        0     4459 2023-06-25 22:40:48.296677 autopack_tools-0.1.1/autopack/get_pack.py
--rw-r--r--   0        0        0     2679 2023-06-23 17:24:04.352595 autopack_tools-0.1.1/autopack/installation.py
--rw-r--r--   0        0        0      794 2023-06-25 23:11:43.009840 autopack_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3455 1970-01-01 00:00:00.000000 autopack_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2920 2023-06-25 23:13:00.716562 autopack_tools-0.1.2/README.md
+-rw-r--r--   0        0        0        6 2023-06-23 17:23:28.293631 autopack_tools-0.1.2/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-23 17:23:28.293676 autopack_tools-0.1.2/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-23 17:23:28.293853 autopack_tools-0.1.2/autopack/__main__.py
+-rw-r--r--   0        0        0     1427 2023-06-25 23:11:09.434943 autopack_tools-0.1.2/autopack/api.py
+-rw-r--r--   0        0        0      864 2023-06-23 17:24:04.323693 autopack_tools-0.1.2/autopack/cli.py
+-rw-r--r--   0        0        0      258 2023-06-23 17:23:28.294559 autopack_tools-0.1.2/autopack/errors.py
+-rw-r--r--   0        0        0     4459 2023-06-25 22:40:48.296677 autopack_tools-0.1.2/autopack/get_pack.py
+-rw-r--r--   0        0        0     2679 2023-06-23 17:24:04.352595 autopack_tools-0.1.2/autopack/installation.py
+-rw-r--r--   0        0        0      796 2023-06-25 23:15:45.962407 autopack_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3481 1970-01-01 00:00:00.000000 autopack_tools-0.1.2/PKG-INFO
```

### Comparing `autopack_tools-0.1.1/README.md` & `autopack_tools-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # AutoPack Tools
 
 [AutoPack](https://autopack.ai) is a repository for tools that are specifically designed for AI Agents.
 
-The `autopack` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
+The `autopack-tools` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
 repository. Tools in AutoPack are called Packs.
 
 ## Note
 
 This is still in the alpha stage. It's roughly at MVP level, and things will not work, features aren't complete, and
 things will change. Be forewarned.
 
 ## Installation
 
-Install the `autopack` package from PyPI using pip:
+Install the `autopack-tools` package from PyPI using pip:
 
 ```bash
-pip install autopack
+pip install autopack-tools
 ```
 
 Or Poetry:
 
 ```bash
-poetry add autopack
+poetry add autopack-tools
 ```
 
 ## Usage
 
 ### Pack IDs
 
 Each pack in the AutoPack repository is identified by a fully qualified path based on its GitHub repository. This format
```

### Comparing `autopack_tools-0.1.1/autopack/api.py` & `autopack_tools-0.1.2/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.1/autopack/cli.py` & `autopack_tools-0.1.2/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.1/autopack/get_pack.py` & `autopack_tools-0.1.2/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.1/autopack/installation.py` & `autopack_tools-0.1.2/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.1/pyproject.toml` & `autopack_tools-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
 
 [tool.poetry.scripts]
 autopack = 'autopack.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
-urllib3 = "^2.0.3"
+urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
```

### Comparing `autopack_tools-0.1.1/PKG-INFO` & `autopack_tools-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package Manager for AI Agent tools
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
-Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Description-Content-Type: text/markdown
 
 # AutoPack Tools
 
 [AutoPack](https://autopack.ai) is a repository for tools that are specifically designed for AI Agents.
 
-The `autopack` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
+The `autopack-tools` Python package is designed to facilitate the installation and usage of tools hosted in the AutoPack
 repository. Tools in AutoPack are called Packs.
 
 ## Note
 
 This is still in the alpha stage. It's roughly at MVP level, and things will not work, features aren't complete, and
 things will change. Be forewarned.
 
 ## Installation
 
-Install the `autopack` package from PyPI using pip:
+Install the `autopack-tools` package from PyPI using pip:
 
 ```bash
-pip install autopack
+pip install autopack-tools
 ```
 
 Or Poetry:
 
 ```bash
-poetry add autopack
+poetry add autopack-tools
 ```
 
 ## Usage
 
 ### Pack IDs
 
 Each pack in the AutoPack repository is identified by a fully qualified path based on its GitHub repository. This format
```

