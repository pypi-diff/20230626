# Comparing `tmp/ocrd-2.8.3.tar.gz` & `tmp/ocrd-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd-2.8.3.tar", last modified: Mon Jun  8 16:56:39 2020, max compression
+gzip compressed data, was "dist/ocrd-2.9.0.tar", last modified: Tue Jun  9 17:33:36 2020, max compression
```

## Comparing `ocrd-2.8.3.tar` & `ocrd-2.9.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:39.000000 ocrd-2.8.3/
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-08 16:56:39.000000 ocrd-2.8.3/setup.cfg
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:39.000000 ocrd-2.8.3/ocrd.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      569 2020-06-08 16:56:39.000000 ocrd-2.8.3/ocrd.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      227 2020-06-08 16:56:38.000000 ocrd-2.8.3/ocrd.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)        5 2020-06-08 16:56:38.000000 ocrd-2.8.3/ocrd.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)      380 2020-06-08 16:56:38.000000 ocrd-2.8.3/ocrd.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-08 16:56:38.000000 ocrd-2.8.3/ocrd.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       81 2020-06-08 16:56:38.000000 ocrd-2.8.3/ocrd.egg-info/entry_points.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)     1086 2020-06-07 19:05:48.000000 ocrd-2.8.3/setup.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      380 2020-06-08 16:56:39.000000 ocrd-2.8.3/PKG-INFO
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:39.000000 ocrd-2.8.3/ocrd/
--rw-rw-r--   0 kba       (1000) kba       (1000)     5853 2020-06-08 11:57:16.000000 ocrd-2.8.3/ocrd/task_sequence.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      841 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/__init__.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:39.000000 ocrd-2.8.3/ocrd/cli/
--rw-rw-r--   0 kba       (1000) kba       (1000)     1824 2020-06-07 19:05:48.000000 ocrd-2.8.3/ocrd/cli/dummy_processor.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4965 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/cli/ocrd_tool.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4661 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/cli/zip.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4893 2020-06-06 19:26:51.000000 ocrd-2.8.3/ocrd/cli/validate.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1760 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/cli/bashlib.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      613 2020-06-07 13:19:20.000000 ocrd-2.8.3/ocrd/cli/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      766 2020-06-08 11:57:16.000000 ocrd-2.8.3/ocrd/cli/process.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    16863 2020-06-08 16:52:58.000000 ocrd-2.8.3/ocrd/cli/workspace.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3615 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/workspace_backup.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    10202 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/workspace_bagger.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     7655 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/resolver.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    39583 2020-06-08 16:52:58.000000 ocrd-2.8.3/ocrd/workspace.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:39.000000 ocrd-2.8.3/ocrd/processor/
--rw-rw-r--   0 kba       (1000) kba       (1000)     7352 2020-06-08 11:57:16.000000 ocrd-2.8.3/ocrd/processor/base.py
--rw-rw-r--   0 kba       (1000) kba       (1000)       97 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/processor/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3568 2020-06-08 11:57:16.000000 ocrd-2.8.3/ocrd/decorators.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      322 2020-05-12 11:01:01.000000 ocrd-2.8.3/ocrd/constants.py
--rw-rw-r--   0 kba       (1000) kba       (1000)       66 2020-05-12 11:01:01.000000 ocrd-2.8.3/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:36.000000 ocrd-2.9.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-09 17:33:36.000000 ocrd-2.9.0/setup.cfg
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:36.000000 ocrd-2.9.0/ocrd.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      585 2020-06-09 17:33:36.000000 ocrd-2.9.0/ocrd.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      227 2020-06-09 17:33:35.000000 ocrd-2.9.0/ocrd.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)        5 2020-06-09 17:33:35.000000 ocrd-2.9.0/ocrd.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      380 2020-06-09 17:33:35.000000 ocrd-2.9.0/ocrd.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-09 17:33:35.000000 ocrd-2.9.0/ocrd.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       81 2020-06-09 17:33:35.000000 ocrd-2.9.0/ocrd.egg-info/entry_points.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1086 2020-06-09 13:50:15.000000 ocrd-2.9.0/setup.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      380 2020-06-09 17:33:36.000000 ocrd-2.9.0/PKG-INFO
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:36.000000 ocrd-2.9.0/ocrd/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     5853 2020-06-09 13:46:06.000000 ocrd-2.9.0/ocrd/task_sequence.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      841 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/__init__.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:36.000000 ocrd-2.9.0/ocrd/cli/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1824 2020-06-09 13:50:15.000000 ocrd-2.9.0/ocrd/cli/dummy_processor.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4965 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/cli/ocrd_tool.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4661 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/cli/zip.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4893 2020-06-06 19:26:51.000000 ocrd-2.9.0/ocrd/cli/validate.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1760 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/cli/bashlib.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      663 2020-06-09 17:08:17.000000 ocrd-2.9.0/ocrd/cli/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      766 2020-06-09 13:46:06.000000 ocrd-2.9.0/ocrd/cli/process.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      927 2020-06-09 17:08:17.000000 ocrd-2.9.0/ocrd/cli/log.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    16863 2020-06-09 17:08:17.000000 ocrd-2.9.0/ocrd/cli/workspace.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3615 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/workspace_backup.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    10202 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/workspace_bagger.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     7655 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/resolver.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    39583 2020-06-09 17:08:17.000000 ocrd-2.9.0/ocrd/workspace.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:36.000000 ocrd-2.9.0/ocrd/processor/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     7352 2020-06-09 13:50:15.000000 ocrd-2.9.0/ocrd/processor/base.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)       97 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/processor/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3568 2020-06-09 13:46:06.000000 ocrd-2.9.0/ocrd/decorators.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      322 2020-05-12 11:01:01.000000 ocrd-2.9.0/ocrd/constants.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)       66 2020-05-12 11:01:01.000000 ocrd-2.9.0/README.md
```

### Comparing `ocrd-2.8.3/ocrd.egg-info/SOURCES.txt` & `ocrd-2.9.0/ocrd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ocrd.egg-info/dependency_links.txt
 ocrd.egg-info/entry_points.txt
 ocrd.egg-info/requires.txt
 ocrd.egg-info/top_level.txt
 ocrd/cli/__init__.py
 ocrd/cli/bashlib.py
 ocrd/cli/dummy_processor.py
+ocrd/cli/log.py
 ocrd/cli/ocrd_tool.py
 ocrd/cli/process.py
 ocrd/cli/validate.py
 ocrd/cli/workspace.py
 ocrd/cli/zip.py
 ocrd/processor/__init__.py
 ocrd/processor/base.py
```

### Comparing `ocrd-2.8.3/setup.py` & `ocrd-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/task_sequence.py` & `ocrd-2.9.0/ocrd/task_sequence.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/__init__.py` & `ocrd-2.9.0/ocrd/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/dummy_processor.py` & `ocrd-2.9.0/ocrd/cli/dummy_processor.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/ocrd_tool.py` & `ocrd-2.9.0/ocrd/cli/ocrd_tool.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/zip.py` & `ocrd-2.9.0/ocrd/cli/zip.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/validate.py` & `ocrd-2.9.0/ocrd/cli/validate.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/bashlib.py` & `ocrd-2.9.0/ocrd/cli/bashlib.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/__init__.py` & `ocrd-2.9.0/ocrd/cli/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ocrd.cli.ocrd_tool import ocrd_tool_cli
 from ocrd.cli.workspace import workspace_cli
 from ocrd.cli.process import process_cli
 from ocrd.cli.bashlib import bashlib_cli
 from ocrd.cli.validate import validate_cli
 from ocrd.decorators import ocrd_loglevel
 from .zip import zip_cli
+from .log import log_cli
 
 @click.group()
 @click.version_option()
 @ocrd_loglevel
 def cli(**kwargs): # pylint: disable=unused-argument
     """
     CLI to OCR-D
@@ -18,7 +19,8 @@
 
 cli.add_command(ocrd_tool_cli)
 cli.add_command(workspace_cli)
 cli.add_command(process_cli)
 cli.add_command(bashlib_cli)
 cli.add_command(zip_cli)
 cli.add_command(validate_cli)
+cli.add_command(log_cli)
```

### Comparing `ocrd-2.8.3/ocrd/cli/process.py` & `ocrd-2.9.0/ocrd/cli/process.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/cli/workspace.py` & `ocrd-2.9.0/ocrd/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/workspace_backup.py` & `ocrd-2.9.0/ocrd/workspace_backup.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/workspace_bagger.py` & `ocrd-2.9.0/ocrd/workspace_bagger.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/resolver.py` & `ocrd-2.9.0/ocrd/resolver.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/workspace.py` & `ocrd-2.9.0/ocrd/workspace.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/processor/base.py` & `ocrd-2.9.0/ocrd/processor/base.py`

 * *Files identical despite different names*

### Comparing `ocrd-2.8.3/ocrd/decorators.py` & `ocrd-2.9.0/ocrd/decorators.py`

 * *Files identical despite different names*

