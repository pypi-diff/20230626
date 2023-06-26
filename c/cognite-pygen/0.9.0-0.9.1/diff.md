# Comparing `tmp/cognite_pygen-0.9.0.tar.gz` & `tmp/cognite_pygen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_pygen-0.9.0.tar", max compression
+gzip compressed data, was "cognite_pygen-0.9.1.tar", max compression
```

## Comparing `cognite_pygen-0.9.0.tar` & `cognite_pygen-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11342 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/LICENSE
--rw-r--r--   0        0        0     5219 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/README.md
--rw-r--r--   0        0        0      140 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/__init__.py
--rw-r--r--   0        0        0     1910 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/data_classes.py
--rw-r--r--   0        0        0     8654 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/__init__.py
--rw-r--r--   0        0        0      167 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19018 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2599 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/get_client.py
--rw-r--r--   0        0        0      399 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-05-22 16:45:26.090266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6507 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     4071 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    19118 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     5941 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7072 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0     3619 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/testing.py
--rw-r--r--   0        0        0     1423 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/py.typed
--rw-r--r--   0        0        0      497 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/dm_clients/settings.toml
--rw-r--r--   0        0        0     1634 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/generator.py
--rw-r--r--   0        0        0     9044 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/main.py
--rw-r--r--   0        0        0      602 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/misc.py
--rw-r--r--   0        0        0     1428 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/parser.py
--rw-r--r--   0        0        0     1346 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/templates/client.txt
--rw-r--r--   0        0        0      819 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/cognite/pygen/version.py
--rw-r--r--   0        0        0     1898 2023-05-22 16:45:26.094266 cognite_pygen-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 cognite_pygen-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5219 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/README.md
+-rw-r--r--   0        0        0      140 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/__init__.py
+-rw-r--r--   0        0        0     1910 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/data_classes.py
+-rw-r--r--   0        0        0     8650 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19018 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3848 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2599 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/get_client.py
+-rw-r--r--   0        0        0      399 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6507 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     4071 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    19118 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     5941 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7072 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     3619 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/testing.py
+-rw-r--r--   0        0        0     1423 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/py.typed
+-rw-r--r--   0        0        0      497 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/dm_clients/settings.toml
+-rw-r--r--   0        0        0     1634 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/generator.py
+-rw-r--r--   0        0        0     9048 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/main.py
+-rw-r--r--   0        0        0      602 2023-06-09 13:21:50.195503 cognite_pygen-0.9.1/cognite/pygen/misc.py
+-rw-r--r--   0        0        0     1428 2023-06-09 13:21:50.199503 cognite_pygen-0.9.1/cognite/pygen/parser.py
+-rw-r--r--   0        0        0     1346 2023-06-09 13:21:50.199503 cognite_pygen-0.9.1/cognite/pygen/templates/client.txt
+-rw-r--r--   0        0        0      819 2023-06-09 13:21:50.199503 cognite_pygen-0.9.1/cognite/pygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-06-09 13:21:50.199503 cognite_pygen-0.9.1/cognite/pygen/version.py
+-rw-r--r--   0        0        0     2207 2023-06-09 13:21:50.199503 cognite_pygen-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 cognite_pygen-0.9.1/PKG-INFO
```

### Comparing `cognite_pygen-0.9.0/LICENSE` & `cognite_pygen-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/README.md` & `cognite_pygen-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/data_classes.py` & `cognite_pygen-0.9.1/cognite/pygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/README.md` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
    DomainModel, e.g. create new pumps, delete a pump, list all pumps...
  * DomainClient - a `dm_clients` term - a Python class (or class instance) which serves as a namespace for easy access
    to all DomainModelAPIs in a use case.
 
 
 ## Installation
 
-1. `pip install cognite-gql-pygen`
+1. `pip install cognite-pygen`
 2. Create a `settings.toml` file, see [settings.toml](./settings.toml) for a template.
    * this step is optional, all settings can be specified in code or via env variables
    * `settings.toml` should contain only things which are safe to commit to git
    * also create `.secrets.toml` and put sensitive settings here
       * the structure of both files (`settings.toml` and `.secrets.toml`) is the same, and the values are merged together
       * example `.secrets.toml`:
         ```toml
```

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/client_dm_v3.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     space: str
     externalId: str
     version: str
     name: Optional[str] = None
     description: Optional[str] = None
     filter: Optional[dict] = None
     implements: Optional[List[dict]] = None
-    properties: dict  # for simplicity, we require this dict to exist, even though the API doesn't
+    properties: Optional[dict] = None
 
 
 class DataModel(DataModelBase):
     space: str
     externalId: str
     version: str
     name: str = ""
```

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/cdf/get_client.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/custom_types/jsonobject.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/custom_types/timestamp.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/domain_client.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/domain_model.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/domain_model_api.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/relationship_api.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/schema.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/domain_modeling/testing.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/domain_modeling/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/dm_clients/misc.py` & `cognite_pygen-0.9.1/cognite/pygen/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/generator.py` & `cognite_pygen-0.9.1/cognite/pygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/main.py` & `cognite_pygen-0.9.1/cognite/pygen/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import inspect
 import subprocess
 import sys
 from contextlib import suppress
 from pathlib import Path
 from typing import Optional
 
-import click
 import toml
 
 try:
+    import click
     import typer
 except ImportError:
     _has_typer = False
     typer = None
 else:
     _has_typer = True
```

### Comparing `cognite_pygen-0.9.0/cognite/pygen/misc.py` & `cognite_pygen-0.9.1/cognite/pygen/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/parser.py` & `cognite_pygen-0.9.1/cognite/pygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/templates/client.txt` & `cognite_pygen-0.9.1/cognite/pygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/cognite/pygen/templates/schema.txt` & `cognite_pygen-0.9.1/cognite/pygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.9.0/pyproject.toml` & `cognite_pygen-0.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-pygen"
-version = "0.9.0"
+version = "0.9.1"
 description = "Cognite GraphQL Python Generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache-2.0"
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
@@ -38,33 +38,34 @@
 cachelib = ">=0.10.2"
 typing-extensions = ">=4.4.0"
 dynaconf = {version=">=3.1.12"}
 toml = {version=">=0.10"}
 
 packaging = {version=">=21.3", optional=true}
 typer = {version = ">=0.9", extras = ["rich"], optional=true }
+mkdocs =  {version="*", optional=true}
+mkdocs-jupyter = {version="*", optional=true}
+mkdocs-material-extensions = {version="*", optional=true}
+mkdocs-git-revision-date-localized-plugin = {version="*", optional=true}
+mkdocs-git-authors-plugin = {version="*", optional=true}
+mkdocs-gitbook = {version="*", optional=true}
 
 [tool.poetry.extras]
 cli = ["packaging", "typer"]
+docs = ["mkdocs", "mkdocs-jupyter", "mkdocs-material-extensions", "mkdocs-git-revision-date-localized-plugin", "mkdocs-git-authors-plugin", "mkdocs-gitbook"]
 all = ["packaging", "typer"]
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pre-commit = "*"
 python-dotenv = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 faker = "*"
-mkdocs = "*"
-mkdocs-jupyter = "*"
-mkdocs-material-extensions = "*"
-mkdocs-git-revision-date-localized-plugin = "*"
-mkdocs-git-authors-plugin = "*"
-mkdocs-gitbook = "*"
 
 [tool.pytest.ini_options]
 filterwarnings = [
   "ignore::DeprecationWarning:pkg_resources",  # TODO check again with dynaconf>=3.2.0 (introduced in setuptools==67.5.0)
 ]
 addopts = "--doctest-modules"
 markers = [
```

### Comparing `cognite_pygen-0.9.0/PKG-INFO` & `cognite_pygen-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: cognite-pygen
-Version: 0.9.0
+Version: 0.9.1
 Summary: Cognite GraphQL Python Generation SDK
 License: Apache-2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: cli
+Provides-Extra: docs
 Requires-Dist: Jinja2 (>=3.1)
 Requires-Dist: cachelib (>=0.10.2)
 Requires-Dist: cognite-sdk (>5.9.0)
 Requires-Dist: dynaconf (>=3.1.12)
 Requires-Dist: graphql-core (>=3.2)
+Requires-Dist: mkdocs ; extra == "docs"
+Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
+Requires-Dist: mkdocs-git-revision-date-localized-plugin ; extra == "docs"
+Requires-Dist: mkdocs-gitbook ; extra == "docs"
+Requires-Dist: mkdocs-jupyter ; extra == "docs"
+Requires-Dist: mkdocs-material-extensions ; extra == "docs"
 Requires-Dist: msal (>=1.16.0)
 Requires-Dist: packaging (>=21.3) ; extra == "cli" or extra == "all"
 Requires-Dist: pydantic (>=1.10)
 Requires-Dist: retry (>=0.9.2)
 Requires-Dist: strawberry-graphql (>=0.156.4,<0.157.0)
 Requires-Dist: toml (>=0.10)
 Requires-Dist: typer[rich] (>=0.9) ; extra == "cli" or extra == "all"
```

