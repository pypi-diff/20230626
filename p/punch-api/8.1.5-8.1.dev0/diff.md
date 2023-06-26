# Comparing `tmp/punch_api-8.1.5.tar.gz` & `tmp/punch_api-8.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punch_api-8.1.5.tar", max compression
+gzip compressed data, was "punch_api-8.1.dev0.tar", max compression
```

## Comparing `punch_api-8.1.5.tar` & `punch_api-8.1.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      477 2023-05-31 12:51:29.000000 punch_api-8.1.5/LICENSE
--rw-r--r--   0        0        0        0 2023-05-31 13:17:54.000000 punch_api-8.1.5/punch_api/__init__.py
--rw-r--r--   0        0        0     1483 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/dag.py
--rw-r--r--   0        0        0      907 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/datasets.py
--rw-r--r--   0        0        0     3759 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/logger.py
--rw-r--r--   0        0        0        0 2023-05-31 13:17:54.000000 punch_api-8.1.5/punch_api/metrics/__init__.py
--rw-r--r--   0        0        0      253 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/metrics/counter.py
--rw-r--r--   0        0        0      372 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/metrics/gauge.py
--rw-r--r--   0        0        0      376 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/metrics/histogram.py
--rw-r--r--   0        0        0     4934 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/metrics/metric_context.py
--rw-r--r--   0        0        0     1960 2023-05-31 12:51:29.000000 punch_api-8.1.5/punch_api/nodes.py
--rw-r--r--   0        0        0      525 2023-06-26 13:21:30.490168 punch_api-8.1.5/pyproject.toml
--rw-r--r--   0        0        0      709 2023-06-26 13:21:31.419205 punch_api-8.1.5/setup.py
--rw-r--r--   0        0        0      500 2023-06-26 13:21:31.419457 punch_api-8.1.5/PKG-INFO
+-rw-r--r--   0        0        0      477 2022-07-07 13:29:26.428205 punch_api-8.1.dev0/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/__init__.py
+-rw-r--r--   0        0        0     1483 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/dag.py
+-rw-r--r--   0        0        0      907 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/datasets.py
+-rw-r--r--   0        0        0     3759 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/logger.py
+-rw-r--r--   0        0        0        0 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/metrics/__init__.py
+-rw-r--r--   0        0        0      253 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/metrics/counter.py
+-rw-r--r--   0        0        0      372 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/metrics/gauge.py
+-rw-r--r--   0        0        0      376 2022-07-07 13:29:26.432205 punch_api-8.1.dev0/punch_api/metrics/histogram.py
+-rw-r--r--   0        0        0     4934 2023-03-09 16:04:33.167967 punch_api-8.1.dev0/punch_api/metrics/metric_context.py
+-rw-r--r--   0        0        0     1960 2023-03-09 16:04:33.267967 punch_api-8.1.dev0/punch_api/nodes.py
+-rw-r--r--   0        0        0      527 2023-03-09 16:07:23.928101 punch_api-8.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0      712 2023-03-09 16:07:24.361938 punch_api-8.1.dev0/setup.py
+-rw-r--r--   0        0        0      503 2023-03-09 16:07:24.362118 punch_api-8.1.dev0/PKG-INFO
```

### Comparing `punch_api-8.1.5/punch_api/dag.py` & `punch_api-8.1.dev0/punch_api/dag.py`

 * *Files identical despite different names*

### Comparing `punch_api-8.1.5/punch_api/datasets.py` & `punch_api-8.1.dev0/punch_api/datasets.py`

 * *Files identical despite different names*

### Comparing `punch_api-8.1.5/punch_api/logger.py` & `punch_api-8.1.dev0/punch_api/logger.py`

 * *Files identical despite different names*

### Comparing `punch_api-8.1.5/punch_api/metrics/metric_context.py` & `punch_api-8.1.dev0/punch_api/metrics/metric_context.py`

 * *Files identical despite different names*

### Comparing `punch_api-8.1.5/punch_api/nodes.py` & `punch_api-8.1.dev0/punch_api/nodes.py`

 * *Files identical despite different names*

### Comparing `punch_api-8.1.5/pyproject.toml` & `punch_api-8.1.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "punch_api"
-version = "8.1.5"
+version = "8.1-dev"
 description = "Punch Python and PySpark Public API"
 authors = ["Punch <contact@punchplatform.com>"]
 maintainers = ["Punch <contact@punchplatform.com>"]
 homepage = "https://punchplatform.com"
 repository = "https://github.com/punchplatform"
 documentation = "https://doc.punchplatform.com"
 include = ["LICENSE"]
```

### Comparing `punch_api-8.1.5/setup.py` & `punch_api-8.1.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['prometheus-client>=0.12.0,<0.13.0']
 
 setup_kwargs = {
     'name': 'punch-api',
-    'version': '8.1.5',
+    'version': '8.1.dev0',
     'description': 'Punch Python and PySpark Public API',
     'long_description': None,
     'author': 'Punch',
     'author_email': 'contact@punchplatform.com',
     'maintainer': 'Punch',
     'maintainer_email': 'contact@punchplatform.com',
     'url': 'https://punchplatform.com',
```

