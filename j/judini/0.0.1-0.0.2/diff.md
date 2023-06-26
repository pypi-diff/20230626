# Comparing `tmp/judini-0.0.1.tar.gz` & `tmp/judini-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judini-0.0.1.tar", last modified: Mon Jun 26 04:18:47 2023, max compression
+gzip compressed data, was "judini-0.0.2.tar", last modified: Mon Jun 26 04:25:04 2023, max compression
```

## Comparing `judini-0.0.1.tar` & `judini-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:18:47.774525 judini-0.0.1/
--rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.1/LICENSE
--rw-r--r--   0 danipower   (501) staff       (20)     1248 2023-06-26 04:18:47.774648 judini-0.0.1/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      752 2023-06-26 04:14:29.000000 judini-0.0.1/README.md
--rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.1/pyproject.toml
--rw-r--r--   0 danipower   (501) staff       (20)      738 2023-06-26 04:18:47.775165 judini-0.0.1/setup.cfg
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:18:47.771010 judini-0.0.1/src/
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:18:47.772925 judini-0.0.1/src/judini/
--rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.1/src/judini/__init__.py
--rw-r--r--   0 danipower   (501) staff       (20)      838 2023-06-26 04:03:43.000000 judini-0.0.1/src/judini/agent.py
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:18:47.774274 judini-0.0.1/src/judini.egg-info/
--rw-r--r--   0 danipower   (501) staff       (20)     1248 2023-06-26 04:18:47.000000 judini-0.0.1/src/judini.egg-info/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:18:47.000000 judini-0.0.1/src/judini.egg-info/SOURCES.txt
--rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:18:47.000000 judini-0.0.1/src/judini.egg-info/dependency_links.txt
--rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:18:47.000000 judini-0.0.1/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.756277 judini-0.0.2/
+-rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.2/LICENSE
+-rw-r--r--   0 danipower   (501) staff       (20)     1177 2023-06-26 04:25:04.756410 judini-0.0.2/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      752 2023-06-26 04:14:29.000000 judini-0.0.2/README.md
+-rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.2/pyproject.toml
+-rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 04:25:04.756916 judini-0.0.2/setup.cfg
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.752291 judini-0.0.2/src/
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.754130 judini-0.0.2/src/judini/
+-rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.2/src/judini/__init__.py
+-rw-r--r--   0 danipower   (501) staff       (20)      836 2023-06-26 04:24:20.000000 judini-0.0.2/src/judini/agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.755980 judini-0.0.2/src/judini.egg-info/
+-rw-r--r--   0 danipower   (501) staff       (20)     1177 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/SOURCES.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/dependency_links.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/top_level.txt
```

### Comparing `judini-0.0.1/LICENSE` & `judini-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `judini-0.0.1/PKG-INFO` & `judini-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.1
+Version: 0.0.2
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `judini-0.0.1/README.md` & `judini-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `judini-0.0.1/setup.cfg` & `judini-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [metadata]
 name = judini
-version = 0.0.1
+version = 0.0.2
 author = Daniel Avila
 author_email = daniel@judini.ai
 description = Judini python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JudiniLabs/judini-python.git
-project_urls = 
-	Bug Tracker = https://github.com/pypa/sampleproject/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `judini-0.0.1/src/judini/agent.py` & `judini-0.0.2/src/judini/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# judini
+# Agent
 import requests
 
-class Judini:
+class Agent:
     def __init__(self, api_key, agent_id):
         self.api_key = api_key
         self.agent_id = agent_id
 
     def set_api_key(self, api_key):
         self.api_key = api_key
```

### Comparing `judini-0.0.1/src/judini.egg-info/PKG-INFO` & `judini-0.0.2/src/judini.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.1
+Version: 0.0.2
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

