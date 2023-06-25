# Comparing `tmp/cstore-0.6.0.tar.gz` & `tmp/cstore-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.6.0.tar", last modified: Sun Jun 25 23:12:10 2023, max compression
+gzip compressed data, was "cstore-0.6.1.tar", last modified: Sun Jun 25 23:20:08 2023, max compression
```

## Comparing `cstore-0.6.0.tar` & `cstore-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.0/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:12:10.754381 cstore-0.6.0/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.6.0/README.md
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/cstore/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.6.0/cstore/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15194 2023-06-25 22:35:01.000000 cstore-0.6.0/cstore/cli.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.0/cstore/constants.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      393 2023-06-21 10:01:53.000000 cstore-0.6.0/cstore/database.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1000 2023-06-25 21:35:45.000000 cstore-0.6.0/cstore/models.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/cstore/repo/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-20 15:21:29.000000 cstore-0.6.0/cstore/repo/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2887 2023-06-25 20:48:02.000000 cstore-0.6.0/cstore/repo/repo_command.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1300 2023-06-25 12:38:12.000000 cstore-0.6.0/cstore/repo/repo_tag.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1758 2023-06-25 21:19:40.000000 cstore-0.6.0/cstore/schemes.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.0/cstore/verbose.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:12:10.754381 cstore-0.6.0/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/entry_points.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-25 23:12:10.000000 cstore-0.6.0/cstore.egg-info/top_level.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      821 2023-06-25 22:53:45.000000 cstore-0.6.0/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-25 23:12:10.754381 cstore-0.6.0/setup.cfg
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.1/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:20:08.144957 cstore-0.6.1/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.6.1/README.md
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/cstore/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.6.1/cstore/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15243 2023-06-25 23:19:03.000000 cstore-0.6.1/cstore/cli.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.1/cstore/constants.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      393 2023-06-21 10:01:53.000000 cstore-0.6.1/cstore/database.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-25 23:16:51.000000 cstore-0.6.1/cstore/models.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/cstore/repo/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-20 15:21:29.000000 cstore-0.6.1/cstore/repo/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2908 2023-06-25 23:16:32.000000 cstore-0.6.1/cstore/repo/repo_command.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1322 2023-06-25 23:16:39.000000 cstore-0.6.1/cstore/repo/repo_tag.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.1/cstore/schemes.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.1/cstore/verbose.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/top_level.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      821 2023-06-25 23:19:11.000000 cstore-0.6.1/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-25 23:20:08.144957 cstore-0.6.1/setup.cfg
```

### Comparing `cstore-0.6.0/LICENSE` & `cstore-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.6.0/PKG-INFO` & `cstore-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.0
+Version: 0.6.1
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cstore-0.6.0/cstore/cli.py` & `cstore-0.6.1/cstore/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from rich.prompt import Prompt
 from rich import print
 from typer import Typer, Option, Exit, Context, confirm, Abort, prompt
 from simple_term_menu import TerminalMenu
 import cryptocode
 
 
-import schemes as schemes
-from models import DcBase, Command, Tag
-from database import engine
-from constants import actions_enum, ActionsEnum
-from repo.repo_command import RepoCommand
-from repo.repo_tag import RepoTag
-from verbose import Verbose
+import cstore.schemes as schemes
+from cstore.models import DcBase, Command, Tag
+from cstore.database import engine
+from cstore.constants import actions_enum, ActionsEnum
+from cstore.repo.repo_command import RepoCommand
+from cstore.repo.repo_tag import RepoTag
+from cstore.verbose import Verbose
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 db_path = "cstore_sqlite.db"
 state = {"verbose": False}
 defult_action = actions_enum.filter
 app = Typer()
 console = Console()
 verbose_manager = Verbose()
```

### Comparing `cstore-0.6.0/cstore/models.py` & `cstore-0.6.1/cstore/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy import Column, Integer, String, ForeignKey, Boolean
 from sqlalchemy.orm import relationship
 
-from database import DcBase
+from cstore.database import DcBase
 
 
 class Command(DcBase):
     __tablename__ = "commands"
     id = Column(Integer, primary_key=True, index=True)
     body = Column(String(500), unique=True, index=True)
     description = Column(String(1000), nullable=True)
```

### Comparing `cstore-0.6.0/cstore/repo/repo_command.py` & `cstore-0.6.1/cstore/repo/repo_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 from sqlalchemy import and_, or_
 
-import schemes as schemes
-from models import Command, Tag, CommandTag
-from database import LocalSession
+import cstore.schemes as schemes
+from cstore.models import Command, Tag, CommandTag
+from cstore.database import LocalSession
 
 
 class RepoCommand:
     def __init__(self) -> None:
         self.db = LocalSession()
 
     def create(self, command_data: schemes.CommandCreateWithTagsSchema) -> Command:
```

### Comparing `cstore-0.6.0/cstore/repo/repo_tag.py` & `cstore-0.6.1/cstore/repo/repo_tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
-import schemes as schemes
-from models import Tag
-from database import LocalSession
+
+import cstore.schemes as schemes
+from cstore.models import Tag
+from cstore.database import LocalSession
 
 
 class RepoTag:
     def __init__(self) -> None:
         self.db = LocalSession()
 
     def create(self, tag_data: schemes.TagSchemaBase) -> Tag:
```

### Comparing `cstore-0.6.0/cstore/schemes.py` & `cstore-0.6.1/cstore/schemes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional, List
-
 from pydantic import validator, root_validator
 from pydantic import BaseModel, Field
 
 
 def to_lowercase(v):
     return str(v).lower()
```

### Comparing `cstore-0.6.0/cstore/verbose.py` & `cstore-0.6.1/cstore/verbose.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.0/cstore.egg-info/PKG-INFO` & `cstore-0.6.1/cstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.0
+Version: 0.6.1
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cstore-0.6.0/pyproject.toml` & `cstore-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cstore"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
     "pydantic",
     "typer[all]",
     "rich",
     "simple_term_menu",
     "SQLAlchemy",
     "pyperclip",
```

