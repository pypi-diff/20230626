# Comparing `tmp/gh_utils-0.6.6.tar.gz` & `tmp/gh_utils-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_utils-0.6.6.tar", max compression
+gzip compressed data, was "gh_utils-0.6.7.tar", max compression
```

## Comparing `gh_utils-0.6.6.tar` & `gh_utils-0.6.7.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1100 2023-03-20 11:20:14.964726 gh_utils-0.6.6/LICENSE
--rw-r--r--   0        0        0     2055 2023-03-20 11:39:20.380308 gh_utils-0.6.6/README.md
--rw-r--r--   0        0        0       90 2023-05-04 16:18:51.488409 gh_utils-0.6.6/gh_utils/__init__.py
--rw-r--r--   0        0        0      609 2023-03-20 11:20:14.965665 gh_utils-0.6.6/gh_utils/config.py
--rwxr-xr-x   0        0        0     5119 2023-05-04 16:16:16.753048 gh_utils-0.6.6/gh_utils/gh_create_repo_and_add_to_remote.py
--rw-r--r--   0        0        0      115 2023-03-20 11:20:14.966076 gh_utils-0.6.6/gh_utils/types.py
--rw-r--r--   0        0        0     1501 2023-03-20 11:20:14.966389 gh_utils-0.6.6/gh_utils/utils.py
--rw-r--r--   0        0        0      806 2023-05-04 16:18:51.487407 gh_utils-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 gh_utils-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-03-20 11:20:14.964726 gh_utils-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2055 2023-03-20 11:39:20.380308 gh_utils-0.6.7/README.md
+-rw-r--r--   0        0        0       90 2023-06-26 15:03:01.792344 gh_utils-0.6.7/gh_utils/__init__.py
+-rw-r--r--   0        0        0      609 2023-03-20 11:20:14.965665 gh_utils-0.6.7/gh_utils/config.py
+-rwxr-xr-x   0        0        0     5134 2023-06-26 14:57:29.474818 gh_utils-0.6.7/gh_utils/gh_create_repo_and_add_to_remote.py
+-rw-r--r--   0        0        0      625 2023-06-26 14:53:40.749514 gh_utils-0.6.7/gh_utils/parse.py
+-rwxr-xr-x   0        0        0     1459 2023-06-26 14:59:56.728420 gh_utils-0.6.7/gh_utils/switch_between_https_and_ssh_remote_types.py
+-rw-r--r--   0        0        0      115 2023-03-20 11:20:14.966076 gh_utils-0.6.7/gh_utils/types.py
+-rw-r--r--   0        0        0     1501 2023-03-20 11:20:14.966389 gh_utils-0.6.7/gh_utils/utils.py
+-rw-r--r--   0        0        0      872 2023-06-26 15:03:01.790894 gh_utils-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 gh_utils-0.6.7/PKG-INFO
```

### Comparing `gh_utils-0.6.6/LICENSE` & `gh_utils-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.6/README.md` & `gh_utils-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.6/gh_utils/config.py` & `gh_utils-0.6.7/gh_utils/config.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.6/gh_utils/gh_create_repo_and_add_to_remote.py` & `gh_utils-0.6.7/gh_utils/gh_create_repo_and_add_to_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 Purpose: gh_create_repo_and_add_to_remote
 """
 
 import argparse
 from functools import cache
 from pathlib import Path
 import subprocess
-from . import __version__
-from .utils import (
+from gh_utils import __version__
+from gh_utils.utils import (
     gh_config_yaml_get_first_hostname_and_username,
     hostname_to_user,
 )
 
 __app_name__ = 'ghcrar'
```

### Comparing `gh_utils-0.6.6/gh_utils/utils.py` & `gh_utils-0.6.7/gh_utils/utils.py`

 * *Files identical despite different names*

### Comparing `gh_utils-0.6.6/pyproject.toml` & `gh_utils-0.6.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "gh-utils"
-version = "0.6.6"
+version = "0.6.7"
 description = "GitHub CLI Utilities"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/gh-utils"
 repository = "https://github.com/tddschn/gh-utils"
 classifiers = ["Topic :: Utilities"]
 keywords = ["gh", "github", "utils"]
 
 [tool.poetry.scripts]
 ghcrar = "gh_utils.gh_create_repo_and_add_to_remote:main"
+ghshs = "gh_utils.switch_between_https_and_ssh_remote_types:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/gh-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyYAML = "^6.0"
```

### Comparing `gh_utils-0.6.6/PKG-INFO` & `gh_utils-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-utils
-Version: 0.6.6
+Version: 0.6.7
 Summary: GitHub CLI Utilities
 Home-page: https://github.com/tddschn/gh-utils
 License: MIT
 Keywords: gh,github,utils
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

