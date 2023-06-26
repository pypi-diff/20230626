# Comparing `tmp/codestamper-0.3.0.tar.gz` & `tmp/codestamper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codestamper-0.3.0.tar", last modified: Wed Aug 17 09:43:17 2022, max compression
+gzip compressed data, was "codestamper-0.3.1.tar", last modified: Mon Jun 26 09:56:33 2023, max compression
```

## Comparing `codestamper-0.3.0.tar` & `codestamper-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-08-17 09:43:17.224022 codestamper-0.3.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1070 2022-08-02 05:52:18.000000 codestamper-0.3.0/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       42 2022-08-12 15:21:55.000000 codestamper-0.3.0/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8025 2022-08-17 09:43:17.224022 codestamper-0.3.0/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7578 2022-08-17 09:07:20.000000 codestamper-0.3.0/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-08-17 09:43:17.224022 codestamper-0.3.0/codestamper/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      144 2022-08-09 21:13:22.000000 codestamper-0.3.0/codestamper/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5989 2022-08-17 08:42:39.000000 codestamper-0.3.0/codestamper/codestamper.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4667 2022-08-09 21:11:27.000000 codestamper-0.3.0/codestamper/gitutils.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3378 2022-08-17 08:38:26.000000 codestamper-0.3.0/codestamper/pythonenv.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-08-17 09:43:17.224022 codestamper-0.3.0/codestamper.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8025 2022-08-17 09:43:17.000000 codestamper-0.3.0/codestamper.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      329 2022-08-17 09:43:17.000000 codestamper-0.3.0/codestamper.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2022-08-17 09:43:17.000000 codestamper-0.3.0/codestamper.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       12 2022-08-17 09:43:17.000000 codestamper-0.3.0/codestamper.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       12 2022-08-17 09:43:17.000000 codestamper-0.3.0/codestamper.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2022-08-08 22:05:01.000000 codestamper-0.3.0/requirements.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2022-08-17 09:43:17.224022 codestamper-0.3.0/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      801 2022-08-17 09:43:03.000000 codestamper-0.3.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 09:56:33.573502 codestamper-0.3.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1070 2023-06-26 09:38:46.000000 codestamper-0.3.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-26 09:38:46.000000 codestamper-0.3.1/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8025 2023-06-26 09:56:33.573502 codestamper-0.3.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7578 2023-06-26 09:38:46.000000 codestamper-0.3.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 09:56:33.573502 codestamper-0.3.1/codestamper/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      144 2023-06-26 09:38:46.000000 codestamper-0.3.1/codestamper/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6379 2023-06-26 09:48:55.000000 codestamper-0.3.1/codestamper/codestamper.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4667 2023-06-26 09:46:03.000000 codestamper-0.3.1/codestamper/gitutils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3600 2023-06-26 09:47:51.000000 codestamper-0.3.1/codestamper/pythonenv.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 09:56:33.573502 codestamper-0.3.1/codestamper.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8025 2023-06-26 09:56:33.000000 codestamper-0.3.1/codestamper.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      349 2023-06-26 09:56:33.000000 codestamper-0.3.1/codestamper.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-26 09:56:33.000000 codestamper-0.3.1/codestamper.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-06-26 09:56:33.000000 codestamper-0.3.1/codestamper.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-06-26 09:56:33.000000 codestamper-0.3.1/codestamper.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-06-26 09:38:46.000000 codestamper-0.3.1/requirements.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-26 09:56:33.573502 codestamper-0.3.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      801 2023-06-26 09:56:17.000000 codestamper-0.3.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-26 09:56:33.573502 codestamper-0.3.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2020 2023-06-26 09:38:46.000000 codestamper-0.3.1/tests/test_basic.py
```

### Comparing `codestamper-0.3.0/LICENSE` & `codestamper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codestamper-0.3.0/PKG-INFO` & `codestamper-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codestamper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Ensure code traceability in ML experiments
 Home-page: https://github.com/bmsan/codestamper
 Author: Bogdan Sandoi
 Author-email: bogdan.sandoi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codestamper-0.3.0/README.md` & `codestamper-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `codestamper-0.3.0/codestamper/codestamper.py` & `codestamper-0.3.1/codestamper/codestamper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import platform
 from datetime import datetime
 import json
 import sys
 import contextlib
+import subprocess
 
 try:
     import pwd  # Used to get username if os.getlogin fails
 except ImportError:
     pass
 
 from typing import List, Union
@@ -15,14 +16,18 @@
 from .gitutils import Git
 
 
 class DirtyWorkspace(Exception):
     """Git Workspace contains modified files and/or untracked files"""
 
 
+class GitUserNotSet(Exception):
+    """Raised when git user/email is not found"""
+
+
 def get_username():
     """
     Returns
     -------
         The system username of the current user
     """
     with contextlib.suppress(Exception):
@@ -96,15 +101,20 @@
             Information related to python packages in conda envs, by default True
 
         """
         state = {"date": datetime.now().strftime("%d/%m/%Y %H:%M:%S")}
         git = state["git"] = {}
         git["hash"] = self.git.get_hash()
         if git_usr:
-            git["user"], git["email"] = self.git.git_user_config()
+            try:
+                git["user"], git["email"] = self.git.git_user_config()
+            except subprocess.CalledProcessError as e:
+                raise GitUserNotSet(
+                    "Could not retrieve git user.name and email. Either set them in your git config or call log_state(...) with git_usr set to False"
+                ) from e
         if node_info:
             node = state["node"] = {}
             node["username"] = get_username()
             uname = platform.uname()
             for key in ["node", "system", "version", "release"]:
                 try:
                     val = getattr(uname, key)
```

### Comparing `codestamper-0.3.0/codestamper/gitutils.py` & `codestamper-0.3.1/codestamper/gitutils.py`

 * *Files identical despite different names*

### Comparing `codestamper-0.3.0/codestamper/pythonenv.py` & `codestamper-0.3.1/codestamper/pythonenv.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,20 @@
         self.pip_deps = None
         self.conda_deps = None
 
     def load_env(self):
         super().load_env()
         if not self.activated:
             return
-        data = subprocess.check_output(["conda", "env", "export"]).decode("utf-8")
+        cmd = ["conda", "env", "export"]
+        try:
+            data = subprocess.check_output(cmd).decode("utf-8")
+        except FileNotFoundError:
+            # On Windows conda command is seen only for shell=True
+            data = subprocess.check_output(' '.join(cmd), shell=True).decode("utf-8")
         self.raw = data
         self.parsed = yaml.safe_load(data)
         self._interpret_deps(self.parsed["dependencies"])
 
     def _interpret_deps(self, data):
         conda_deps = {}
         pip_deps = {}
```

### Comparing `codestamper-0.3.0/codestamper.egg-info/PKG-INFO` & `codestamper-0.3.1/codestamper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codestamper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Ensure code traceability in ML experiments
 Home-page: https://github.com/bmsan/codestamper
 Author: Bogdan Sandoi
 Author-email: bogdan.sandoi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codestamper-0.3.0/setup.py` & `codestamper-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="codestamper",
-    version="0.3.0",
+    version="0.3.1",
     author="Bogdan Sandoi",
     author_email="bogdan.sandoi@gmail.com",
     description=("Ensure code traceability in ML experiments"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=("tests",)),
     classifiers=[
```

