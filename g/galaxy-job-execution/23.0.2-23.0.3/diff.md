# Comparing `tmp/galaxy-job-execution-23.0.2.tar.gz` & `tmp/galaxy-job-execution-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_execution/dist/.tmp-x8if9q6x/galaxy-job-execution-23.0.2.tar", last modified: Tue Jun 13 17:11:21 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_execution/dist/.tmp-njhylgn6/galaxy-job-execution-23.0.3.tar", last modified: Mon Jun 26 09:54:53 2023, max compression
```

## Comparing `galaxy-job-execution-23.0.2.tar` & `galaxy-job-execution-23.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-job-execution-23.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/actions/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/actions/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/compute_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/container_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/output_collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/ports/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/ports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/ports/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/job_execution/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/metadata/set_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-13 17:11:21.000000 galaxy-job-execution-23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-job-execution-23.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-job-execution-23.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/actions/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/compute_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/container_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/output_collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/ports/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/ports/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/job_execution/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/metadata/set_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-26 09:54:53.000000 galaxy-job-execution-23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:48:33.000000 galaxy-job-execution-23.0.3/test-requirements.txt
```

### Comparing `galaxy-job-execution-23.0.2/LICENSE` & `galaxy-job-execution-23.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/PKG-INFO` & `galaxy-job-execution-23.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/actions/post.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/actions/post.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/compute_environment.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/compute_environment.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/container_monitor.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/container_monitor.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/datasets.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/output_collect.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/output_collect.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/ports/view.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/ports/view.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/job_execution/setup.py` & `galaxy-job-execution-23.0.3/galaxy/job_execution/setup.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/metadata/__init__.py` & `galaxy-job-execution-23.0.3/galaxy/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy/metadata/set_metadata.py` & `galaxy-job-execution-23.0.3/galaxy/metadata/set_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/PKG-INFO` & `galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-job-execution-23.0.2/galaxy_job_execution.egg-info/SOURCES.txt` & `galaxy-job-execution-23.0.3/galaxy_job_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.0.2/setup.cfg` & `galaxy-job-execution-23.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-job-execution
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.2
+version = 23.0.3
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-files
 	galaxy-objectstore
```

