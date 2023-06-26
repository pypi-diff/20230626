# Comparing `tmp/gh_utils-0.6.7.tar.gz` & `tmp/gh_utils-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_utils-0.6.7.tar", max compression
+gzip compressed data, was "gh_utils-0.6.8.tar", max compression
```

## Comparing `gh_utils-0.6.7.tar` & `gh_utils-0.6.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1100 2023-03-20 11:20:14.964726 gh_utils-0.6.7/LICENSE
--rw-r--r--   0        0        0     2055 2023-03-20 11:39:20.380308 gh_utils-0.6.7/README.md
--rw-r--r--   0        0        0       90 2023-06-26 15:03:01.792344 gh_utils-0.6.7/gh_utils/__init__.py
--rw-r--r--   0        0        0      609 2023-03-20 11:20:14.965665 gh_utils-0.6.7/gh_utils/config.py
--rwxr-xr-x   0        0        0     5134 2023-06-26 14:57:29.474818 gh_utils-0.6.7/gh_utils/gh_create_repo_and_add_to_remote.py
--rw-r--r--   0        0        0      625 2023-06-26 14:53:40.749514 gh_utils-0.6.7/gh_utils/parse.py
--rwxr-xr-x   0        0        0     1459 2023-06-26 14:59:56.728420 gh_utils-0.6.7/gh_utils/switch_between_https_and_ssh_remote_types.py
--rw-r--r--   0        0        0      115 2023-03-20 11:20:14.966076 gh_utils-0.6.7/gh_utils/types.py
--rw-r--r--   0        0        0     1501 2023-03-20 11:20:14.966389 gh_utils-0.6.7/gh_utils/utils.py
--rw-r--r--   0        0        0      872 2023-06-26 15:03:01.790894 gh_utils-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 gh_utils-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-03-20 11:20:14.964726 gh_utils-0.6.8/LICENSE
+-rw-r--r--   0        0        0     2642 2023-06-26 15:07:40.170202 gh_utils-0.6.8/README.md
+-rw-r--r--   0        0        0       90 2023-06-26 15:08:11.890921 gh_utils-0.6.8/gh_utils/__init__.py
+-rw-r--r--   0        0        0      609 2023-03-20 11:20:14.965665 gh_utils-0.6.8/gh_utils/config.py
+-rwxr-xr-x   0        0        0     5134 2023-06-26 14:57:29.474818 gh_utils-0.6.8/gh_utils/gh_create_repo_and_add_to_remote.py
+-rw-r--r--   0        0        0      625 2023-06-26 14:53:40.749514 gh_utils-0.6.8/gh_utils/parse.py
+-rwxr-xr-x   0        0        0     1459 2023-06-26 14:59:56.728420 gh_utils-0.6.8/gh_utils/switch_between_https_and_ssh_remote_types.py
+-rw-r--r--   0        0        0      115 2023-03-20 11:20:14.966076 gh_utils-0.6.8/gh_utils/types.py
+-rw-r--r--   0        0        0     1501 2023-03-20 11:20:14.966389 gh_utils-0.6.8/gh_utils/utils.py
+-rw-r--r--   0        0        0      872 2023-06-26 15:08:11.890381 gh_utils-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 gh_utils-0.6.8/PKG-INFO
```

### Comparing `gh_utils-0.6.7/LICENSE` & `gh_utils-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.7/gh_utils/config.py` & `gh_utils-0.6.8/gh_utils/config.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.7/gh_utils/gh_create_repo_and_add_to_remote.py` & `gh_utils-0.6.8/gh_utils/gh_create_repo_and_add_to_remote.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.7/gh_utils/parse.py` & `gh_utils-0.6.8/gh_utils/parse.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.7/gh_utils/switch_between_https_and_ssh_remote_types.py` & `gh_utils-0.6.8/gh_utils/switch_between_https_and_ssh_remote_types.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.7/gh_utils/utils.py` & `gh_utils-0.6.8/gh_utils/utils.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.7/pyproject.toml` & `gh_utils-0.6.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gh-utils"
-version = "0.6.7"
+version = "0.6.8"
 description = "GitHub CLI Utilities"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/gh-utils"
 repository = "https://github.com/tddschn/gh-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `gh_utils-0.6.7/PKG-INFO` & `gh_utils-0.6.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-utils
-Version: 0.6.7
+Version: 0.6.8
 Summary: GitHub CLI Utilities
 Home-page: https://github.com/tddschn/gh-utils
 License: MIT
 Keywords: gh,github,utils
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -27,14 +27,17 @@
     - [pipx](#pipx)
     - [pip](#pip)
   - [Utilities](#utilities)
     - [ghcrar](#ghcrar)
       - [Features](#features)
       - [Usage](#usage)
       - [Screenshots](#screenshots)
+    - [ghshs](#ghshs)
+      - [Usage](#usage-1)
+      - [Screenshot](#screenshot)
   - [Develop](#develop)
 
 ## Installation
 
 ### pipx
 
 This is the recommended installation method.
@@ -88,14 +91,41 @@
 #### Screenshots
 
 ![ghcrar-public](images/ghcrar-public.png)
 
 ![](images/ghcrar-dupe-url-and-set-default.png)
 
 
+### ghshs
+
+<!-- cSpell:disable -->
+**gh** **s**witch between **h**ttps and **s**sh
+<!-- cSpell:enable -->
+
+#### Usage
+
+```
+$ ghshs --help
+
+usage: ghshs [-h] [-r REMOTE] [-V]
+
+Switch between HTTPS and SSH types of GitHub remotes
+
+options:
+  -h, --help            show this help message and exit
+  -r REMOTE, --remote REMOTE
+                        Name of the remote to switch (default: origin)
+  -V, --version         show program's version number and exit
+
+```
+
+#### Screenshot
+
+![](./images/ghshs.png)
+
 ## Develop
 
 ```
 $ git clone https://github.com/tddschn/gh-utils.git
 $ cd gh-utils
 $ poetry install
 ```
```

