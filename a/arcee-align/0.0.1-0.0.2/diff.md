# Comparing `tmp/arcee-align-0.0.1.tar.gz` & `tmp/arcee-align-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcee-align-0.0.1.tar", last modified: Mon Jun 26 04:17:10 2023, max compression
+gzip compressed data, was "arcee-align-0.0.2.tar", last modified: Mon Jun 26 04:36:13 2023, max compression
```

## Comparing `arcee-align-0.0.1.tar` & `arcee-align-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:17:10.788679 arcee-align-0.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2152 2023-06-26 04:17:10.788679 arcee-align-0.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2023-06-25 17:41:45.000000 arcee-align-0.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:17:10.772679 arcee-align-0.0.1/arcee/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-25 23:36:58.000000 arcee-align-0.0.1/arcee/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:17:10.776679 arcee-align-0.0.1/arcee/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-06-25 23:31:22.000000 arcee-align-0.0.1/arcee/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5076 2023-06-25 23:39:47.000000 arcee-align-0.0.1/arcee/data/generate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2262 2023-06-26 03:23:40.000000 arcee-align-0.0.1/arcee/data/instruction_set.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:17:10.780679 arcee-align-0.0.1/arcee/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-06-22 05:12:31.000000 arcee-align-0.0.1/arcee/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-26 03:23:40.000000 arcee-align-0.0.1/arcee/models/lm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:17:10.788679 arcee-align-0.0.1/arcee_align.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2152 2023-06-26 04:17:10.000000 arcee-align-0.0.1/arcee_align.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-06-26 04:17:10.000000 arcee-align-0.0.1/arcee_align.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 04:17:10.000000 arcee-align-0.0.1/arcee_align.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-06-26 04:17:10.000000 arcee-align-0.0.1/arcee_align.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-26 04:17:10.000000 arcee-align-0.0.1/arcee_align.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 04:17:10.788679 arcee-align-0.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1136 2023-06-26 04:17:02.000000 arcee-align-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.652157 arcee-align-0.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2152 2023-06-26 04:36:13.652157 arcee-align-0.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2023-06-25 17:41:45.000000 arcee-align-0.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.636157 arcee-align-0.0.2/arcee/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-26 04:36:09.000000 arcee-align-0.0.2/arcee/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.640157 arcee-align-0.0.2/arcee/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-06-25 23:31:22.000000 arcee-align-0.0.2/arcee/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5076 2023-06-25 23:39:47.000000 arcee-align-0.0.2/arcee/data/generate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2262 2023-06-26 03:23:40.000000 arcee-align-0.0.2/arcee/data/instruction_set.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.644157 arcee-align-0.0.2/arcee/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-06-22 05:12:31.000000 arcee-align-0.0.2/arcee/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-26 03:23:40.000000 arcee-align-0.0.2/arcee/models/lm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 04:36:13.648157 arcee-align-0.0.2/arcee_align.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2152 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-26 04:36:13.000000 arcee-align-0.0.2/arcee_align.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 04:36:13.652157 arcee-align-0.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1136 2023-06-26 04:17:02.000000 arcee-align-0.0.2/setup.py
```

### Comparing `arcee-align-0.0.1/PKG-INFO` & `arcee-align-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-align
-Version: 0.0.1
+Version: 0.0.2
 Summary: The open source toolkit for finetuning and deploying LLMs
 Home-page: https://arcee.ai/
 Author: Arcee
 Author-email: jacob@arcee.ai
 License: UNKNOWN
 Description: # Arcee
```

### Comparing `arcee-align-0.0.1/README.md` & `arcee-align-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.1/arcee/data/generate.py` & `arcee-align-0.0.2/arcee/data/generate.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.1/arcee/data/instruction_set.py` & `arcee-align-0.0.2/arcee/data/instruction_set.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.1/arcee/models/lm.py` & `arcee-align-0.0.2/arcee/models/lm.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.1/arcee_align.egg-info/PKG-INFO` & `arcee-align-0.0.2/arcee_align.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-align
-Version: 0.0.1
+Version: 0.0.2
 Summary: The open source toolkit for finetuning and deploying LLMs
 Home-page: https://arcee.ai/
 Author: Arcee
 Author-email: jacob@arcee.ai
 License: UNKNOWN
 Description: # Arcee
```

### Comparing `arcee-align-0.0.1/setup.py` & `arcee-align-0.0.2/setup.py`

 * *Files identical despite different names*

