# Comparing `tmp/transformersplus-0.0.1.tar.gz` & `tmp/transformersplus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformersplus-0.0.1.tar", last modified: Wed Jun 21 09:30:29 2023, max compression
+gzip compressed data, was "transformersplus-0.1.1.tar", last modified: Mon Jun 26 10:29:49 2023, max compression
```

## Comparing `transformersplus-0.0.1.tar` & `transformersplus-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.233898 transformersplus-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 09:30:18.000000 transformersplus-0.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.225898 transformersplus-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.229898 transformersplus-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 09:30:18.000000 transformersplus-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-21 09:30:18.000000 transformersplus-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-21 09:30:18.000000 transformersplus-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-21 09:30:29.233898 transformersplus-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 09:30:18.000000 transformersplus-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.225898 transformersplus-0.0.1/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.229898 transformersplus-0.0.1/example/albert/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-21 09:30:18.000000 transformersplus-0.0.1/example/albert/bright_albet.runtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-21 09:30:18.000000 transformersplus-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:30:29.233898 transformersplus-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.229898 transformersplus-0.0.1/transformersplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.229898 transformersplus-0.0.1/transformersplus/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.233898 transformersplus-0.0.1/transformersplus/models/bright_albert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/models/bright_albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    61119 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/models/bright_albert/modeling_bright_albert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.233898 transformersplus-0.0.1/transformersplus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:18.000000 transformersplus-0.0.1/transformersplus/utils/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:30:29.229898 transformersplus-0.0.1/transformersplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-21 09:30:29.000000 transformersplus-0.0.1/transformersplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 09:30:29.000000 transformersplus-0.0.1/transformersplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:30:29.000000 transformersplus-0.0.1/transformersplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 09:30:29.000000 transformersplus-0.0.1/transformersplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 09:30:29.000000 transformersplus-0.0.1/transformersplus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 10:29:33.000000 transformersplus-0.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.054513 transformersplus-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.058513 transformersplus-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 10:29:33.000000 transformersplus-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-26 10:29:33.000000 transformersplus-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-26 10:29:33.000000 transformersplus-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-26 10:29:49.066514 transformersplus-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 10:29:33.000000 transformersplus-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.054513 transformersplus-0.1.1/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.062513 transformersplus-0.1.1/example/albert/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86634 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 10:29:33.000000 transformersplus-0.1.1/example/albert/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-26 10:29:33.000000 transformersplus-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:29:49.066514 transformersplus-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.062513 transformersplus-0.1.1/transformersplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus/models/bright_albert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/bright_albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61119 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/models/bright_albert/modeling_bright_albert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-26 10:29:33.000000 transformersplus-0.1.1/transformersplus/utils/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:29:49.066514 transformersplus-0.1.1/transformersplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 10:29:49.000000 transformersplus-0.1.1/transformersplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 10:29:48.000000 transformersplus-0.1.1/transformersplus.egg-info/top_level.txt
```

### Comparing `transformersplus-0.0.1/.github/workflows/python-publish.yml` & `transformersplus-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `transformersplus-0.0.1/.gitignore` & `transformersplus-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `transformersplus-0.0.1/LICENSE` & `transformersplus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transformersplus-0.0.1/PKG-INFO` & `transformersplus-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformersplus
-Version: 0.0.1
+Version: 0.1.1
 Summary: Add Some plus features to transformers.
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/msclock/transformersplus.git
 Project-URL: Source, https://github.com/msclock/transformersplus.git
 Project-URL: Tracker, https://github.com/msclock/transformersplus/issues
 Keywords: machine-learning,deep-learning,transformers,inference,pytorch,vision,nlp
 Classifier: Development Status :: 4 - Beta
```

### Comparing `transformersplus-0.0.1/pyproject.toml` & `transformersplus-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 [tool.distutils.bdist_wheel]
 python_tag = "py37.py38.py39.py310"
 
 [tool.setuptools.packages.find]
 namespaces = false
 
 [tool.setuptools.package-data]
-yolov5_utils = ["**/*"]
+transformersplus = ["**/*"]
 
 [tool.setuptools.dynamic]
 version = { attr = "transformersplus.__version__.__version__" }
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
```

### Comparing `transformersplus-0.0.1/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py` & `transformersplus-0.1.1/transformersplus/models/bright_albert/convert_bright_albert_origin_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformersplus-0.0.1/transformersplus/models/bright_albert/modeling_bright_albert.py` & `transformersplus-0.1.1/transformersplus/models/bright_albert/modeling_bright_albert.py`

 * *Files identical despite different names*

### Comparing `transformersplus-0.0.1/transformersplus.egg-info/PKG-INFO` & `transformersplus-0.1.1/transformersplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformersplus
-Version: 0.0.1
+Version: 0.1.1
 Summary: Add Some plus features to transformers.
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/msclock/transformersplus.git
 Project-URL: Source, https://github.com/msclock/transformersplus.git
 Project-URL: Tracker, https://github.com/msclock/transformersplus/issues
 Keywords: machine-learning,deep-learning,transformers,inference,pytorch,vision,nlp
 Classifier: Development Status :: 4 - Beta
```

### Comparing `transformersplus-0.0.1/transformersplus.egg-info/SOURCES.txt` & `transformersplus-0.1.1/transformersplus.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
-example/albert/bright_albet.runtest.py
+example/albert/.gitignore
+example/albert/README.md
+example/albert/app.py
+example/albert/image.png
+example/albert/optimize.py
+example/albert/requirements.txt
 transformersplus/__init__.py
 transformersplus/__version__.py
 transformersplus.egg-info/PKG-INFO
 transformersplus.egg-info/SOURCES.txt
 transformersplus.egg-info/dependency_links.txt
 transformersplus.egg-info/requires.txt
 transformersplus.egg-info/top_level.txt
```

