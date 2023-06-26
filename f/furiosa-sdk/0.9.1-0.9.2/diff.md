# Comparing `tmp/furiosa_sdk-0.9.1.tar.gz` & `tmp/furiosa_sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa_sdk-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "furiosa_sdk-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `furiosa_sdk-0.9.1.tar` & `furiosa_sdk-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      386 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/Makefile
--rw-r--r--   0        0        0     2627 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/README.md
--rw-r--r--   0        0        0     1107 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/docs/Makefile
--rw-r--r--   0        0        0     5330 2023-05-24 05:34:31.472839 furiosa_sdk-0.9.1/docs/conf.py
--rw-r--r--   0        0        0      670 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/docs/furiosa.rst
--rw-r--r--   0        0        0      470 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/docs/index.rst
--rw-r--r--   0        0        0      795 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/docs/make.bat
--rw-r--r--   0        0        0       18 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/furiosa/sdk/__init__.py
--rw-r--r--   0        0        0     1829 2023-05-24 05:34:31.476839 furiosa_sdk-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 furiosa_sdk-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/Makefile
+-rw-r--r--   0        0        0     2627 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/README.md
+-rw-r--r--   0        0        0     1107 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/docs/Makefile
+-rw-r--r--   0        0        0     5330 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/docs/conf.py
+-rw-r--r--   0        0        0      670 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/docs/furiosa.rst
+-rw-r--r--   0        0        0      470 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-02 07:36:53.164978 furiosa_sdk-0.9.2/docs/make.bat
+-rw-r--r--   0        0        0       18 2023-06-02 07:36:53.168979 furiosa_sdk-0.9.2/furiosa/sdk/__init__.py
+-rw-r--r--   0        0        0     1829 2023-06-26 05:41:26.717925 furiosa_sdk-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 furiosa_sdk-0.9.2/PKG-INFO
```

### Comparing `furiosa_sdk-0.9.1/README.md` & `furiosa_sdk-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `furiosa_sdk-0.9.1/docs/Makefile` & `furiosa_sdk-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `furiosa_sdk-0.9.1/docs/conf.py` & `furiosa_sdk-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furiosa_sdk-0.9.1/docs/furiosa.rst` & `furiosa_sdk-0.9.2/docs/furiosa.rst`

 * *Files identical despite different names*

### Comparing `furiosa_sdk-0.9.1/docs/make.bat` & `furiosa_sdk-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `furiosa_sdk-0.9.1/pyproject.toml` & `furiosa_sdk-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "furiosa-sdk"
-version = "0.9.1"
+version = "0.9.2"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `furiosa_sdk-0.9.1/PKG-INFO` & `furiosa_sdk-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Furiosa SDK
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

