# Comparing `tmp/hyko_sdk-0.1.7.tar.gz` & `tmp/hyko_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.1.7.tar", last modified: Sun Jun 25 10:43:50 2023, max compression
+gzip compressed data, was "hyko_sdk-0.1.8.tar", last modified: Mon Jun 26 11:56:27 2023, max compression
```

## Comparing `hyko_sdk-0.1.7.tar` & `hyko_sdk-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/PKG-INFO
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      411 2023-05-17 08:56:51.000000 hyko_sdk-0.1.7/README.md
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/hyko_sdk/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       40 2023-06-21 11:17:29.000000 hyko_sdk-0.1.7/hyko_sdk/__init__.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)     2915 2023-06-25 10:41:00.000000 hyko_sdk-0.1.7/hyko_sdk/io.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)     2798 2023-06-25 10:39:49.000000 hyko_sdk-0.1.7/hyko_sdk/metadata.py
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/hyko_sdk.egg-info/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      250 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        1 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/requires.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/top_level.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       80 2023-06-21 11:17:29.000000 hyko_sdk-0.1.7/pyproject.toml
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      327 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/setup.cfg
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/PKG-INFO
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      411 2023-05-17 08:56:51.000000 hyko_sdk-0.1.8/README.md
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/hyko_sdk/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       60 2023-06-26 11:54:14.000000 hyko_sdk-0.1.8/hyko_sdk/__init__.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      682 2023-06-26 11:51:00.000000 hyko_sdk-0.1.8/hyko_sdk/error.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)     4785 2023-06-26 11:53:34.000000 hyko_sdk-0.1.8/hyko_sdk/io.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)     2791 2023-06-26 11:49:05.000000 hyko_sdk-0.1.8/hyko_sdk/metadata.py
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/hyko_sdk.egg-info/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      268 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        1 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       37 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/requires.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-26 11:56:27.000000 hyko_sdk-0.1.8/hyko_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       80 2023-06-21 11:17:29.000000 hyko_sdk-0.1.8/pyproject.toml
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      357 2023-06-26 11:56:27.066570 hyko_sdk-0.1.8/setup.cfg
```

### Comparing `hyko_sdk-0.1.7/hyko_sdk/metadata.py` & `hyko_sdk-0.1.8/hyko_sdk/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from typing import Any, List, Union, Optional
+from typing import Any, List, Optional
 from .io import IOPortType, IOPort
 
 
 def pmodel_to_ports(pmodel: BaseModel) -> List[IOPort]:
     
     schema = pmodel.schema()
```

