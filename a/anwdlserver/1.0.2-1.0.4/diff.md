# Comparing `tmp/anwdlserver-1.0.2.tar.gz` & `tmp/anwdlserver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anwdlserver-1.0.2.tar", last modified: Mon Jun 26 19:56:16 2023, max compression
+gzip compressed data, was "anwdlserver-1.0.4.tar", last modified: Mon Jun 26 20:27:34 2023, max compression
```

## Comparing `anwdlserver-1.0.2.tar` & `anwdlserver-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:16.293060 anwdlserver-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/CONTRIBUTING
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44508 2023-06-26 19:56:16.289060 anwdlserver-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:16.289060 anwdlserver-1.0.2/anwdlserver/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:16.289060 anwdlserver-1.0.2/anwdlserver/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/core/virtualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:16.289060 anwdlserver-1.0.2/anwdlserver/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/anwdlserver/tools/accesstk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:16.289060 anwdlserver-1.0.2/anwdlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44508 2023-06-26 19:56:16.000000 anwdlserver-1.0.2/anwdlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-26 19:56:16.000000 anwdlserver-1.0.2/anwdlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:56:16.000000 anwdlserver-1.0.2/anwdlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 19:56:16.000000 anwdlserver-1.0.2/anwdlserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 19:56:16.000000 anwdlserver-1.0.2/anwdlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 19:56:16.000000 anwdlserver-1.0.2/anwdlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:56:16.289060 anwdlserver-1.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/resources/anweddol-server.service
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/resources/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:56:16.293060 anwdlserver-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-26 19:56:06.000000 anwdlserver-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/CONTRIBUTING
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44508 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/anwdlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/anwdlserver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/core/virtualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/anwdlserver/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/anwdlserver/tools/accesstk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/anwdlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44508 2023-06-26 20:27:34.000000 anwdlserver-1.0.4/anwdlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-26 20:27:34.000000 anwdlserver-1.0.4/anwdlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:27:34.000000 anwdlserver-1.0.4/anwdlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 20:27:34.000000 anwdlserver-1.0.4/anwdlserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 20:27:34.000000 anwdlserver-1.0.4/anwdlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 20:27:34.000000 anwdlserver-1.0.4/anwdlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/resources/anweddol-server.service
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/resources/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:27:34.423325 anwdlserver-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-26 20:27:24.000000 anwdlserver-1.0.4/setup.py
```

### Comparing `anwdlserver-1.0.2/CONTRIBUTING` & `anwdlserver-1.0.4/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/LICENSE` & `anwdlserver-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/PKG-INFO` & `anwdlserver-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anwdlserver
-Version: 1.0.2
+Version: 1.0.4
 Summary: The Anweddol server implementation
 Home-page: https://github.com/the-anweddol-project/Anweddol-server
 Author: The Anweddol project
 Author-email: The Anweddol project <the-anweddol-project@proton.me>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `anwdlserver-1.0.2/README.md` & `anwdlserver-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/cli.py` & `anwdlserver-1.0.4/anwdlserver/cli.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/config.py` & `anwdlserver-1.0.4/anwdlserver/config.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/client.py` & `anwdlserver-1.0.4/anwdlserver/core/client.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/crypto.py` & `anwdlserver-1.0.4/anwdlserver/core/crypto.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/database.py` & `anwdlserver-1.0.4/anwdlserver/core/database.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/sanitize.py` & `anwdlserver-1.0.4/anwdlserver/core/sanitize.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/server.py` & `anwdlserver-1.0.4/anwdlserver/core/server.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/util.py` & `anwdlserver-1.0.4/anwdlserver/core/util.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/core/virtualization.py` & `anwdlserver-1.0.4/anwdlserver/core/virtualization.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/process.py` & `anwdlserver-1.0.4/anwdlserver/process.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver/tools/accesstk.py` & `anwdlserver-1.0.4/anwdlserver/tools/accesstk.py`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/anwdlserver.egg-info/PKG-INFO` & `anwdlserver-1.0.4/anwdlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anwdlserver
-Version: 1.0.2
+Version: 1.0.4
 Summary: The Anweddol server implementation
 Home-page: https://github.com/the-anweddol-project/Anweddol-server
 Author: The Anweddol project
 Author-email: The Anweddol project <the-anweddol-project@proton.me>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `anwdlserver-1.0.2/anwdlserver.egg-info/SOURCES.txt` & `anwdlserver-1.0.4/anwdlserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/pyproject.toml` & `anwdlserver-1.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tools.setuptools]
 packages = ["anwdlserver", "anwdlserver.core", "anwdlserver.tools"]
 
 [project]
 name = "anwdlserver"
-version = "1.0.2"
+version = "1.0.4"
 description = "The Anweddol server implementation"
 authors = [
   { name="The Anweddol project", email="the-anweddol-project@proton.me" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -22,15 +22,14 @@
   "Topic :: System :: Emulators",
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 dependencies = [
   "cryptography",
   "paramiko",
-  "requests",
   "python-daemon",
   "cerberus",
   "defusedxml",
   "sqlalchemy",
   "pyyaml",
 ]
```

### Comparing `anwdlserver-1.0.2/resources/config.yaml` & `anwdlserver-1.0.4/resources/config.yaml`

 * *Files identical despite different names*

### Comparing `anwdlserver-1.0.2/setup.py` & `anwdlserver-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     print(
         "[SETUP] WARN : Non-root user detected, the installation limits to the 'anwdlserver' python package installation"
     )
 
 print("[SETUP] Installing Anweddol server package ...")
 setup(
     name="anwdlserver",
-    version="1.0.3",
+    version="1.0.4",
     description="The Anweddol server implementation",
     author="The Anweddol project",
     author_email="the-anweddol-project@proton.me",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Intended Audience :: Developers",
@@ -93,15 +93,14 @@
     ],
     license="GPL v3",
     url="https://github.com/the-anweddol-project/Anweddol-server",
     packages=["anwdlserver", "anwdlserver.core", "anwdlserver.tools"],
     install_requires=[
         "cryptography",
         "paramiko",
-        "requests",
         "python-daemon",
         "cerberus",
         "defusedxml",
         "sqlalchemy",
         "pyyaml",
     ],
     include_package_data=True,
```

