# Comparing `tmp/type_infer-0.0.7.tar.gz` & `tmp/type_infer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "type_infer-0.0.7.tar", max compression
+gzip compressed data, was "type_infer-0.0.9.tar", max compression
```

## Comparing `type_infer-0.0.7.tar` & `type_infer-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35104 2022-11-03 09:26:29.975913 type_infer-0.0.7/LICENSE
--rw-r--r--   0        0        0     1778 2022-11-03 09:26:29.975913 type_infer-0.0.7/README.md
--rw-r--r--   0        0        0      551 2022-11-03 09:26:29.975913 type_infer-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      206 2022-11-03 09:26:29.979913 type_infer-0.0.7/type_infer/__init__.py
--rw-r--r--   0        0        0     1213 2022-11-03 09:26:29.979913 type_infer-0.0.7/type_infer/base.py
--rw-r--r--   0        0        0     2304 2022-11-03 09:26:29.979913 type_infer-0.0.7/type_infer/dtype.py
--rw-r--r--   0        0        0     7004 2022-11-03 09:26:29.979913 type_infer-0.0.7/type_infer/helpers.py
--rw-r--r--   0        0        0    15529 2022-11-03 09:26:29.979913 type_infer-0.0.7/type_infer/infer.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 type_infer-0.0.7/setup.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 type_infer-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35104 2022-11-18 21:07:46.504644 type_infer-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1778 2022-11-18 21:07:46.504644 type_infer-0.0.9/README.md
+-rw-r--r--   0        0        0      551 2022-11-18 21:07:46.508644 type_infer-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      206 2022-11-18 21:07:46.512644 type_infer-0.0.9/type_infer/__init__.py
+-rw-r--r--   0        0        0     1213 2022-11-18 21:07:46.512644 type_infer-0.0.9/type_infer/base.py
+-rw-r--r--   0        0        0     2304 2022-11-18 21:07:46.512644 type_infer-0.0.9/type_infer/dtype.py
+-rw-r--r--   0        0        0     7054 2022-11-18 21:07:46.512644 type_infer-0.0.9/type_infer/helpers.py
+-rw-r--r--   0        0        0    15549 2022-11-18 21:07:46.512644 type_infer-0.0.9/type_infer/infer.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 type_infer-0.0.9/setup.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 type_infer-0.0.9/PKG-INFO
```

### Comparing `type_infer-0.0.7/LICENSE` & `type_infer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `type_infer-0.0.7/README.md` & `type_infer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `type_infer-0.0.7/pyproject.toml` & `type_infer-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "type_infer"
-version = "0.0.7"
+version = "0.0.9"
 description = "Automated type inference for Machine Learning pipelines."
 authors = ["MindsDB Inc. <hello@mindsdb.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "type_infer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `type_infer-0.0.7/type_infer/base.py` & `type_infer-0.0.9/type_infer/base.py`

 * *Files identical despite different names*

### Comparing `type_infer-0.0.7/type_infer/dtype.py` & `type_infer-0.0.9/type_infer/dtype.py`

 * *Files identical despite different names*

### Comparing `type_infer-0.0.7/type_infer/helpers.py` & `type_infer-0.0.9/type_infer/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,15 @@
         nr_words += len(tokens)
         for tok in tokens_no_stop:
             word_dist[tok] += 1
 
     return nr_words, dict(word_dist), dict(nr_words_dist)
 
 
+# @TODO: eventually move these into .helpers.text
 def tokenize_text(text):
     return [t.lower() for t in nltk.word_tokenize(decontracted(text)) if contains_alnum(t)]
 
 
 def decontracted(phrase):
     # specific
     phrase = re.sub(r"won\'t", "will not", phrase)
```

### Comparing `type_infer-0.0.7/type_infer/infer.py` & `type_infer-0.0.9/type_infer/infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             return False, None
         else:
             nr_map.add(numeric_bit)
 
         if char_const is None:
             char_const = char_part
 
-        if char_part is None or char_part != char_const:
+        if char_part is None or char_part == '-' or char_part != char_const:
             return False, None
 
     if len(nr_map) > 20 and len(nr_map) > len(col_data) / 200:
         return True, {char_const: {
             'multiplier': 1
         }}
     else:
```

### Comparing `type_infer-0.0.7/setup.py` & `type_infer-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pandas>=1,<2',
  'python-dateutil>=2.1,<3.0',
  'scipy>=1,<2',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'type-infer',
-    'version': '0.0.7',
+    'version': '0.0.9',
     'description': 'Automated type inference for Machine Learning pipelines.',
     'long_description': '# MindsDB Type Infer\n<h1 align="center">\n\t<img width="300" src="https://github.com/mindsdb/mindsdb_native/blob/stable/assets/MindsDBColorPurp@3x.png?raw=true" alt="MindsDB">\n\t<br>\n\n</h1>\n<div align="center">\n\t<a href="https://github.com/mindsdb/type_infer/actions/workflows/python-package.yml"><img src="https://github.com/mindsdb/type_infer/actions/workflows/python-package.yml/badge.svg?branch=stable" alt="Type Infer workflow"></a>\n  <a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.8.x|%203.9.x-brightgreen.svg" alt="Python supported"></a>\n  <a href="https://badge.fury.io/py/type-infer"><img src="https://badge.fury.io/py/type-infer.svg" alt="PyPI version" height="18"></a>\n<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/type-infer">  \n    <a href="https://join.slack.com/t/mindsdbcommunity/shared_invite/zt-o8mrmx3l-5ai~5H66s6wlxFfBMVI6wQ" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>\n\t</br>\n\t\n  <h3 align="center">\n    <a href="https://www.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Website</a>\n    <span> | </span>\n    <a href="https://mindsdb.github.io/type_infer/">Docs</a>\n    <span> | </span>\n    <a href="https://join.slack.com/t/mindsdbcommunity/shared_invite/zt-o8mrmx3l-5ai~5H66s6wlxFfBMVI6wQ">Community Slack</a>\n    <span> | </span>\n    <a href="https://github.com/mindsdb/mindsdb/projects">Contribute</a>\n    <span> | </span>\n    <a href="https://mindsdb.com/hacktoberfest">Hacktoberfest</a>\n  </h3>\n  \n</div>\nAutomated type inference for Machine Learning pipelines.\n\n# Documentation\n<a href="https://mindsdb.github.io/type_infer">Documentation link</a>\n',
     'author': 'MindsDB Inc.',
     'author_email': 'hello@mindsdb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['type_infer'] package_data = \ {'': ['*']} install_requires = \
 ['colorlog>=6.5.0,<7.0.0', 'dataclasses-json>=0.5.4,<0.6.0',
 'langid>=1.1.6,<2.0.0', 'nltk>=3,<4', 'numpy>=1.15,<2.0', 'pandas>=1,<2',
 'python-dateutil>=2.1,<3.0', 'scipy>=1,<2', 'toml>=0.10.2,<0.11.0']
-setup_kwargs = { 'name': 'type-infer', 'version': '0.0.7', 'description':
+setup_kwargs = { 'name': 'type-infer', 'version': '0.0.9', 'description':
 'Automated type inference for Machine Learning pipelines.', 'long_description':
 '# MindsDB Type Infer\n
                            ****** \n\t[MindsDB]\n\t
                                   \n\n ******
 \n
    \n\t[Type_Infer_workflow]\n [Python_supported]\n [PyPI_version]\n[PyPI -
                   Downloads] \n [MindsDB_Community]\n\t\n\t\n
```

### Comparing `type_infer-0.0.7/PKG-INFO` & `type_infer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: type-infer
-Version: 0.0.7
+Version: 0.0.9
 Summary: Automated type inference for Machine Learning pipelines.
 License: GPL-3.0
 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: type-infer Version: 0.0.7 Summary: Automated type
+Metadata-Version: 2.1 Name: type-infer Version: 0.0.9 Summary: Automated type
 inference for Machine Learning pipelines. License: GPL-3.0 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com Requires-Python: >=3.7,<3.10 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Dist: colorlog (>=6.5.0,<7.0.0)
 Requires-Dist: dataclasses-json (>=0.5.4,<0.6.0) Requires-Dist: langid
```

