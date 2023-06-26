# Comparing `tmp/judini-0.0.4.tar.gz` & `tmp/judini-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judini-0.0.4.tar", last modified: Mon Jun 26 04:48:55 2023, max compression
+gzip compressed data, was "judini-0.0.5.tar", last modified: Mon Jun 26 05:01:20 2023, max compression
```

## Comparing `judini-0.0.4.tar` & `judini-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.091369 judini-0.0.4/
--rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.4/LICENSE
--rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 04:48:55.091489 judini-0.0.4/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)     1019 2023-06-26 04:48:43.000000 judini-0.0.4/README.md
--rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.4/pyproject.toml
--rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 04:48:55.092002 judini-0.0.4/setup.cfg
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.087473 judini-0.0.4/src/
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.089578 judini-0.0.4/src/judini/
--rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.4/src/judini/__init__.py
--rw-r--r--   0 danipower   (501) staff       (20)     1131 2023-06-26 04:48:06.000000 judini-0.0.4/src/judini/agent.py
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.091131 judini-0.0.4/src/judini.egg-info/
--rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/SOURCES.txt
--rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/dependency_links.txt
--rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.091215 judini-0.0.5/
+-rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.5/LICENSE
+-rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 05:01:20.091335 judini-0.0.5/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)     1019 2023-06-26 04:48:43.000000 judini-0.0.5/README.md
+-rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 05:00:34.000000 judini-0.0.5/pyproject.toml
+-rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 05:01:20.091892 judini-0.0.5/setup.cfg
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.087888 judini-0.0.5/src/
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.089483 judini-0.0.5/src/judini/
+-rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.5/src/judini/__init__.py
+-rw-r--r--   0 danipower   (501) staff       (20)     1331 2023-06-26 04:59:30.000000 judini-0.0.5/src/judini/agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.090905 judini-0.0.5/src/judini.egg-info/
+-rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/SOURCES.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/dependency_links.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/top_level.txt
```

### Comparing `judini-0.0.4/LICENSE` & `judini-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `judini-0.0.4/PKG-INFO` & `judini-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.4
+Version: 0.0.5
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `judini-0.0.4/README.md` & `judini-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `judini-0.0.4/setup.cfg` & `judini-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = judini
-version = 0.0.4
+version = 0.0.5
 author = Daniel Avila
 author_email = daniel@judini.ai
 description = Judini python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JudiniLabs/judini-python.git
 classifiers =
```

### Comparing `judini-0.0.4/src/judini.egg-info/PKG-INFO` & `judini-0.0.5/src/judini.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.4
+Version: 0.0.5
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

