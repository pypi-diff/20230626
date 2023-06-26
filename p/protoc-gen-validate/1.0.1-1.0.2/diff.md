# Comparing `tmp/protoc-gen-validate-1.0.1.tar.gz` & `tmp/protoc-gen-validate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoc-gen-validate-1.0.1.tar", last modified: Tue May  9 19:00:48 2023, max compression
+gzip compressed data, was "protoc-gen-validate-1.0.2.tar", last modified: Mon Jun 26 16:36:01 2023, max compression
```

## Comparing `protoc-gen-validate-1.0.1.tar` & `protoc-gen-validate-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:00:48.898105 protoc-gen-validate-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-05-09 19:00:47.000000 protoc-gen-validate-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1730 2023-05-09 19:00:48.898105 protoc-gen-validate-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-09 18:56:31.000000 protoc-gen-validate-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:00:48.898105 protoc-gen-validate-1.0.1/protoc_gen_validate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 18:56:31.000000 protoc-gen-validate-1.0.1/protoc_gen_validate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50287 2023-05-09 18:56:31.000000 protoc-gen-validate-1.0.1/protoc_gen_validate/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:00:48.898105 protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1730 2023-05-09 19:00:48.000000 protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-09 19:00:48.000000 protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 19:00:48.000000 protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-09 19:00:48.000000 protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 19:00:48.000000 protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-09 18:56:31.000000 protoc-gen-validate-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-09 19:00:48.902106 protoc-gen-validate-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    31250 2023-05-09 19:00:47.000000 protoc-gen-validate-1.0.1/validate.proto
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:01.033677 protoc-gen-validate-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-26 16:36:00.000000 protoc-gen-validate-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-26 16:36:01.033677 protoc-gen-validate-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-26 16:32:57.000000 protoc-gen-validate-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:01.033677 protoc-gen-validate-1.0.2/protoc_gen_validate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 16:32:57.000000 protoc-gen-validate-1.0.2/protoc_gen_validate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50287 2023-06-26 16:32:57.000000 protoc-gen-validate-1.0.2/protoc_gen_validate/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:36:01.033677 protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-26 16:36:00.000000 protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-26 16:36:01.000000 protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:36:00.000000 protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-26 16:36:00.000000 protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 16:36:00.000000 protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-26 16:32:57.000000 protoc-gen-validate-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-26 16:36:01.033677 protoc-gen-validate-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    31250 2023-06-26 16:36:00.000000 protoc-gen-validate-1.0.2/validate.proto
```

### Comparing `protoc-gen-validate-1.0.1/LICENSE` & `protoc-gen-validate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-1.0.1/PKG-INFO` & `protoc-gen-validate-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoc-gen-validate
-Version: 1.0.1
+Version: 1.0.2
 Summary: PGV for python via just-in-time code generation
 Home-page: https://github.com/bufbuild/protoc-gen-validate
 Author: Buf
 Author-email: dev@buf.build
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `protoc-gen-validate-1.0.1/README.md` & `protoc-gen-validate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-1.0.1/protoc_gen_validate/validator.py` & `protoc-gen-validate-1.0.2/protoc_gen_validate/validator.py`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-1.0.1/protoc_gen_validate.egg-info/PKG-INFO` & `protoc-gen-validate-1.0.2/protoc_gen_validate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoc-gen-validate
-Version: 1.0.1
+Version: 1.0.2
 Summary: PGV for python via just-in-time code generation
 Home-page: https://github.com/bufbuild/protoc-gen-validate
 Author: Buf
 Author-email: dev@buf.build
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `protoc-gen-validate-1.0.1/setup.cfg` & `protoc-gen-validate-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `protoc-gen-validate-1.0.1/validate.proto` & `protoc-gen-validate-1.0.2/validate.proto`

 * *Files identical despite different names*

