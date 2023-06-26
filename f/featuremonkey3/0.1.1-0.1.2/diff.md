# Comparing `tmp/featuremonkey3-0.1.1.tar.gz` & `tmp/featuremonkey3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuremonkey3-0.1.1.tar", max compression
+gzip compressed data, was "featuremonkey3-0.1.2.tar", max compression
```

## Comparing `featuremonkey3-0.1.1.tar` & `featuremonkey3-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1055 2023-05-12 15:29:33.644059 featuremonkey3-0.1.1/LICENSE
--rw-r--r--   0        0        0      617 2023-05-12 15:29:33.644059 featuremonkey3-0.1.1/README.rst
--rw-r--r--   0        0        0      647 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/__init__.py
--rw-r--r--   0        0        0    12720 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/composer.py
--rw-r--r--   0        0        0     1017 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/helpers.py
--rw-r--r--   0        0        0     5556 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/importhooks.py
--rw-r--r--   0        0        0      578 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/composer_mocks.py
--rw-r--r--   0        0        0      251 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testmodule1.py
--rw-r--r--   0        0        0        7 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testmodule2.py
--rw-r--r--   0        0        0        0 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testmodule3.py
--rw-r--r--   0        0        0       63 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testpackage1/__init__.py
--rw-r--r--   0        0        0       32 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testpackage1/submodule.py
--rw-r--r--   0        0        0     9729 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/test_composer.py
--rw-r--r--   0        0        0        0 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/__init__.py
--rw-r--r--   0        0        0      742 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/helper.py
--rw-r--r--   0        0        0     2292 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/logger.py
--rw-r--r--   0        0        0     4871 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/serializer.py
--rw-r--r--   0        0        0      499 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 featuremonkey3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-11 20:07:53.200629 featuremonkey3-0.1.2/LICENSE
+-rw-r--r--   0        0        0      617 2023-04-21 20:54:01.547095 featuremonkey3-0.1.2/README.rst
+-rw-r--r--   0        0        0      647 2023-05-11 19:54:48.923937 featuremonkey3-0.1.2/featuremonkey3/__init__.py
+-rw-r--r--   0        0        0    12720 2023-05-12 15:33:24.210206 featuremonkey3-0.1.2/featuremonkey3/composer.py
+-rw-r--r--   0        0        0     1017 2023-04-21 20:54:01.550951 featuremonkey3-0.1.2/featuremonkey3/helpers.py
+-rw-r--r--   0        0        0     5556 2023-05-12 15:33:24.210720 featuremonkey3-0.1.2/featuremonkey3/importhooks.py
+-rw-r--r--   0        0        0      578 2023-05-11 19:58:45.820594 featuremonkey3-0.1.2/featuremonkey3/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:54:01.551531 featuremonkey3-0.1.2/featuremonkey3/test/mock/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-12 15:33:24.211041 featuremonkey3-0.1.2/featuremonkey3/test/mock/composer_mocks.py
+-rw-r--r--   0        0        0      251 2023-04-21 20:54:01.551769 featuremonkey3-0.1.2/featuremonkey3/test/mock/testmodule1.py
+-rw-r--r--   0        0        0        7 2023-04-21 20:54:01.551863 featuremonkey3-0.1.2/featuremonkey3/test/mock/testmodule2.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:54:01.551904 featuremonkey3-0.1.2/featuremonkey3/test/mock/testmodule3.py
+-rw-r--r--   0        0        0       63 2023-04-21 20:54:01.552097 featuremonkey3-0.1.2/featuremonkey3/test/mock/testpackage1/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-27 14:03:41.570693 featuremonkey3-0.1.2/featuremonkey3/test/mock/testpackage1/submodule.py
+-rw-r--r--   0        0        0     9729 2023-05-12 15:33:24.211369 featuremonkey3-0.1.2/featuremonkey3/test/test_composer.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:54:01.552286 featuremonkey3-0.1.2/featuremonkey3/tracing/__init__.py
+-rw-r--r--   0        0        0      742 2023-04-21 20:54:01.552444 featuremonkey3-0.1.2/featuremonkey3/tracing/helper.py
+-rw-r--r--   0        0        0     2292 2023-04-21 20:54:01.552672 featuremonkey3-0.1.2/featuremonkey3/tracing/logger.py
+-rw-r--r--   0        0        0     4871 2023-04-21 20:54:01.552827 featuremonkey3-0.1.2/featuremonkey3/tracing/serializer.py
+-rw-r--r--   0        0        0      501 2023-06-26 21:56:24.716699 featuremonkey3-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 featuremonkey3-0.1.2/PKG-INFO
```

### Comparing `featuremonkey3-0.1.1/LICENSE` & `featuremonkey3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/README.rst` & `featuremonkey3-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/__init__.py` & `featuremonkey3-0.1.2/featuremonkey3/__init__.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/composer.py` & `featuremonkey3-0.1.2/featuremonkey3/composer.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/helpers.py` & `featuremonkey3-0.1.2/featuremonkey3/helpers.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/importhooks.py` & `featuremonkey3-0.1.2/featuremonkey3/importhooks.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/test/__init__.py` & `featuremonkey3-0.1.2/featuremonkey3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/test/mock/composer_mocks.py` & `featuremonkey3-0.1.2/featuremonkey3/test/mock/composer_mocks.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/test/test_composer.py` & `featuremonkey3-0.1.2/featuremonkey3/test/test_composer.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/tracing/helper.py` & `featuremonkey3-0.1.2/featuremonkey3/tracing/helper.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/tracing/logger.py` & `featuremonkey3-0.1.2/featuremonkey3/tracing/logger.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/featuremonkey3/tracing/serializer.py` & `featuremonkey3-0.1.2/featuremonkey3/tracing/serializer.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.1/PKG-INFO` & `featuremonkey3-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: featuremonkey3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python 3.11 compatible fork of featuremonkey, a Python FOP framework first developed by Hendrik Speidel.
 License: MIT
 Author: Adrian Wong
 Author-email: adrianwong227@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/x-rst
 
 featuremonkey - FOP for Python
 ==================================
 
 .. image:: https://secure.travis-ci.org/henzk/featuremonkey.png
```

