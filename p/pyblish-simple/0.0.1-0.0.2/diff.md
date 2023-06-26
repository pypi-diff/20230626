# Comparing `tmp/pyblish-simple-0.0.1.tar.gz` & `tmp/pyblish-simple-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblish-simple-0.0.1.tar", last modified: Mon Jun 26 12:16:46 2023, max compression
+gzip compressed data, was "pyblish-simple-0.0.2.tar", last modified: Mon Jun 26 12:23:57 2023, max compression
```

## Comparing `pyblish-simple-0.0.1.tar` & `pyblish-simple-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:16:46.650183 pyblish-simple-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:16:46.646183 pyblish-simple-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:16:46.646183 pyblish-simple-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 12:16:46.650183 pyblish-simple-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:16:46.646183 pyblish-simple-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   145457 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/docs/screen1.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:16:46.650183 pyblish-simple-0.0.1/pyblish_simple/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/pyblish_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/pyblish_simple/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:16:46.650183 pyblish-simple-0.0.1/pyblish_simple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 12:16:46.000000 pyblish-simple-0.0.1/pyblish_simple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 12:16:46.000000 pyblish-simple-0.0.1/pyblish_simple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:16:46.000000 pyblish-simple-0.0.1/pyblish_simple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 12:16:46.000000 pyblish-simple-0.0.1/pyblish_simple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 12:16:46.000000 pyblish-simple-0.0.1/pyblish_simple.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 12:16:33.000000 pyblish-simple-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:16:46.650183 pyblish-simple-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:23:57.860018 pyblish-simple-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   145457 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/docs/screen1.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/pyblish_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/pyblish_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/pyblish_simple/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/pyblish_simple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-26 12:23:57.000000 pyblish-simple-0.0.2/pyblish_simple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 12:23:57.000000 pyblish-simple-0.0.2/pyblish_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:23:57.000000 pyblish-simple-0.0.2/pyblish_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 12:23:57.000000 pyblish-simple-0.0.2/pyblish_simple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 12:23:57.000000 pyblish-simple-0.0.2/pyblish_simple.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 12:23:44.000000 pyblish-simple-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:23:57.864018 pyblish-simple-0.0.2/setup.cfg
```

### Comparing `pyblish-simple-0.0.1/.github/workflows/python-publish.yml` & `pyblish-simple-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyblish-simple-0.0.1/docs/README.md` & `pyblish-simple-0.0.2/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyblish-simple
 A Pyblish GUI trying to be more 'intuitive' than [pyblish lite](https://github.com/pyblish/pyblish-lite) & [pyblish-qml](https://github.com/pyblish/pyblish-qml)
 
 ## Limitations
 ⚠️ It was designed for validating instances, and currently doesn't show context, export or publish plugins.
 
-![](/docs/screen1.jpg)
+![docs/screen1.jpg](https://raw.githubusercontent.com/hannesdelbeke/pyblish-simple/main/docs/screen1.jpg)
 _left pyblish_lite, right pyblish_simple_
 
 ## How to use
 ### Users
 - Collected instances show on the left 
 - Select an instance to show relevant validations in the bottom right
 - Select a validation to show it's description in the top right
@@ -65,9 +65,8 @@
   - [ ] research how to show context plugins
   - [ ] research how to show export and publish plugins
 
 PR-s are welcome.
 
 ## community
 - [Pyblish forum thread](https://forums.pyblish.com/t/pyblish-simple-a-new-ui-aimed-at-artists/701)
-
-
+- PYPI https://pypi.org/project/pyblish-simple/
```

### Comparing `pyblish-simple-0.0.1/docs/screen1.jpg` & `pyblish-simple-0.0.2/docs/screen1.jpg`

 * *Files identical despite different names*

### Comparing `pyblish-simple-0.0.1/pyblish_simple/view.py` & `pyblish-simple-0.0.2/pyblish_simple/view.py`

 * *Files identical despite different names*

### Comparing `pyblish-simple-0.0.1/pyproject.toml` & `pyblish-simple-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 [project]
 name = "pyblish-simple"
 authors = [
     {name = "Hannes"},
 ]
 description = "a GUI for pyblish, to see which instance failed and why"
-readme = "README.md"
+readme = "docs/README.md"
 requires-python = ">=3.4"
 keywords = ["plugin", "pyblish", "add-on", "extension", "manager", "studio", "dcc", "app", "application", "artist"]
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"', "Qt.py", "pyblish"]
 #dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

