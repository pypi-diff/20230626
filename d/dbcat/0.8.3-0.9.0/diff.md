# Comparing `tmp/dbcat-0.8.3.tar.gz` & `tmp/dbcat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbcat-0.8.3.tar", last modified: Tue Nov  9 06:52:05 2021, max compression
+gzip compressed data, was "dbcat-0.9.0.tar", last modified: Mon Nov 15 12:35:50 2021, max compression
```

## Comparing `dbcat-0.8.3.tar` & `dbcat-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0     1063 2021-11-09 06:51:49.822855 dbcat-0.8.3/LICENSE
--rw-r--r--   0        0        0     1467 2021-11-09 06:51:49.822855 dbcat-0.8.3/README.md
--rw-r--r--   0        0        0     3091 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/__init__.py
--rw-r--r--   0        0        0     3844 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/__main__.py
--rw-r--r--   0        0        0     2179 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/alembic.ini
--rw-r--r--   0        0        0      122 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/catalog/__init__.py
--rw-r--r--   0        0        0    15650 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/catalog/catalog.py
--rw-r--r--   0        0        0    12428 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/catalog/db.py
--rw-r--r--   0        0        0    12045 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/catalog/models.py
--rw-r--r--   0        0        0     4737 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/catalog/sqlite_extractor.py
--rw-r--r--   0        0        0      177 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/log_mixin.py
--rw-r--r--   0        0        0      477 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/__init__.py
--rw-r--r--   0        0        0     2430 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/env.py
--rw-r--r--   0        0        0      494 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/script.py.mako
--rw-r--r--   0        0        0      819 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/versions/3509a9f07432_add_athena_columns.py
--rw-r--r--   0        0        0     2222 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/versions/477d6d4b6ad7_add_update_create_columns.py
--rw-r--r--   0        0        0      806 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/versions/7d2638f2ab5f_add_tasks_table.py
--rw-r--r--   0        0        0        0 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/versions/__init__.py
--rw-r--r--   0        0        0     5475 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/versions/d1daff1715f7_initial_run.py
--rw-r--r--   0        0        0     3146 2021-11-09 06:51:49.822855 dbcat-0.8.3/dbcat/migrations/versions/d2c711b84996_add_pii_type_enum_to_column.py
--rw-r--r--   0        0        0     1541 2021-11-09 06:51:49.826855 dbcat-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2652 2021-11-09 06:52:05.929329 dbcat-0.8.3/setup.py
--rw-r--r--   0        0        0     2875 2021-11-09 06:52:05.930012 dbcat-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-11-15 12:35:34.344251 dbcat-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1467 2021-11-15 12:35:34.344251 dbcat-0.9.0/README.md
+-rw-r--r--   0        0        0       38 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/__init__.py
+-rw-r--r--   0        0        0     2054 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/__main__.py
+-rw-r--r--   0        0        0     2179 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/alembic.ini
+-rw-r--r--   0        0        0     4176 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/amundsen.py
+-rw-r--r--   0        0        0     2410 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/api.py
+-rw-r--r--   0        0        0      110 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/app_state.py
+-rw-r--r--   0        0        0      122 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/catalog/__init__.py
+-rw-r--r--   0        0        0    15645 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/catalog/catalog.py
+-rw-r--r--   0        0        0    12428 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/catalog/db.py
+-rw-r--r--   0        0        0    12045 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/catalog/models.py
+-rw-r--r--   0        0        0     4737 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/catalog/sqlite_extractor.py
+-rw-r--r--   0        0        0     8570 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/cli.py
+-rw-r--r--   0        0        0     2277 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/generators.py
+-rw-r--r--   0        0        0      477 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/migrations/__init__.py
+-rw-r--r--   0        0        0     2430 2021-11-15 12:35:34.344251 dbcat-0.9.0/dbcat/migrations/env.py
+-rw-r--r--   0        0        0      494 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/script.py.mako
+-rw-r--r--   0        0        0      819 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/versions/3509a9f07432_add_athena_columns.py
+-rw-r--r--   0        0        0     2222 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/versions/477d6d4b6ad7_add_update_create_columns.py
+-rw-r--r--   0        0        0      806 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/versions/7d2638f2ab5f_add_tasks_table.py
+-rw-r--r--   0        0        0        0 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     5475 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/versions/d1daff1715f7_initial_run.py
+-rw-r--r--   0        0        0     3146 2021-11-15 12:35:34.348251 dbcat-0.9.0/dbcat/migrations/versions/d2c711b84996_add_pii_type_enum_to_column.py
+-rw-r--r--   0        0        0     1550 2021-11-15 12:35:34.348251 dbcat-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2675 2021-11-15 12:35:50.934774 dbcat-0.9.0/setup.py
+-rw-r--r--   0        0        0     2913 2021-11-15 12:35:50.935102 dbcat-0.9.0/PKG-INFO
```

### Comparing `dbcat-0.8.3/LICENSE` & `dbcat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/README.md` & `dbcat-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/__init__.py` & `dbcat-0.9.0/dbcat/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,84 @@
-# flake8: noqa
-
-__version__ = "0.8.2"
-
 import logging
+from enum import Enum
 from typing import List, Optional
 
 import yaml
 from alembic import command
 
 from dbcat.catalog import Catalog
 from dbcat.catalog.catalog import PGCatalog, SqliteCatalog
 from dbcat.catalog.db import DbScanner
-from dbcat.log_mixin import LogMixin
 from dbcat.migrations import get_alembic_config
 
 LOGGER = logging.getLogger(__name__)
 
 
+class OutputFormat(str, Enum):
+    tabular = "tabular"
+    json = "json"
+
+
 def catalog_connection(
-    catalog_path: str = None,
-    catalog_host: str = None,
-    catalog_port: int = None,
-    catalog_user: str = None,
-    catalog_password: str = None,
-    catalog_database: str = None,
+    path: str = None,
+    host: str = None,
+    port: int = None,
+    user: str = None,
+    password: str = None,
+    database: str = None,
 ) -> Catalog:
     if (
-        catalog_host is not None
-        and catalog_port is not None
-        and catalog_user is not None
-        and catalog_password is not None
-        and catalog_database is not None
+        host is not None
+        and user is not None
+        and password is not None
+        and database is not None
     ):
         return PGCatalog(
-            host=catalog_host,
-            port=str(catalog_port),
-            user=catalog_user,
-            password=catalog_password,
-            database=catalog_database,
+            host=host, port=port, user=user, password=password, database=database,
         )
-    elif catalog_path is not None:
-        return SqliteCatalog(path=str(catalog_path))
+    elif path is not None:
+        return SqliteCatalog(path=str(path))
 
     raise AttributeError("None of Path or Postgres connection parameters are provided")
 
 
 def catalog_connection_yaml(config: str) -> Catalog:
     config_yaml = yaml.safe_load(config)
-    if "path" in config_yaml["catalog"]:
-        return SqliteCatalog(**config_yaml["catalog"])
-    else:
-        return PGCatalog(**config_yaml["catalog"])
+    return catalog_connection(**config_yaml["catalog"])
 
 
 def init_db(catalog_obj: Catalog) -> None:
     """
     Initialize database
     """
     LOGGER.info("Initializing the database")
 
     config = get_alembic_config(catalog_obj.engine)
     LOGGER.debug(config)
     command.upgrade(config, "heads")
 
 
-def add_connections(catalog_obj: Catalog, config: str) -> None:
-    config_yaml = yaml.safe_load(config)
-
-    with catalog_obj.managed_session:
-        for conn in config_yaml["connections"]:
-            LOGGER.info("Adding {}".format(conn))
-            catalog_obj.add_source(**conn)
-
-
-def pull(
-    catalog_obj: Catalog,
-    connection_name: str,
-    include_schema_regex_str: Optional[List[str]] = None,
-    exclude_schema_regex_str: Optional[List[str]] = None,
-    include_table_regex_str: Optional[List[str]] = None,
-    exclude_table_regex_str: Optional[List[str]] = None,
-) -> None:
-    with catalog_obj.managed_session:
-        source = catalog_obj.get_source(connection_name)
-        LOGGER.debug("Source: {}".format(source))
-        scanner = DbScanner(
-            catalog_obj,
-            source,
-            include_schema_regex_str=include_schema_regex_str,
-            exclude_schema_regex_str=exclude_schema_regex_str,
-            include_table_regex_str=include_table_regex_str,
-            exclude_table_regex_str=exclude_table_regex_str,
-        )
-        LOGGER.info("Scanning {}".format(scanner.name))
-        scanner.scan()
-
-
-def pull_all(catalog_obj: Catalog) -> None:
-    with catalog_obj.managed_session:
-        for source in catalog_obj.get_sources():
-            LOGGER.info("Starting scan on {}".format(source))
-            pull(catalog_obj, source.name)
+def scan_sources(
+    catalog: Catalog,
+    source_names: Optional[List[str]] = None,
+    include_schema_regex: Optional[List[str]] = None,
+    exclude_schema_regex: Optional[List[str]] = None,
+    include_table_regex: Optional[List[str]] = None,
+    exclude_table_regex: Optional[List[str]] = None,
+):
+    with catalog.managed_session:
+        if source_names is not None and len(source_names) > 0:
+            sources = [catalog.get_source(source_name) for source_name in source_names]
+        else:
+            sources = catalog.get_sources()
+
+        for source in sources:
+            scanner = DbScanner(
+                catalog,
+                source,
+                include_schema_regex_str=include_schema_regex,
+                exclude_schema_regex_str=exclude_schema_regex,
+                include_table_regex_str=include_table_regex,
+                exclude_table_regex_str=exclude_table_regex,
+            )
+            LOGGER.info("Scanning {}".format(scanner.name))
+            scanner.scan()
```

### Comparing `dbcat-0.8.3/dbcat/alembic.ini` & `dbcat-0.9.0/dbcat/alembic.ini`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/catalog/catalog.py` & `dbcat-0.9.0/dbcat/catalog/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,22 +427,22 @@
 class PGCatalog(Catalog):
     def __init__(
         self,
         user: str,
         password: str,
         database: str,
         host: str,
-        port: str = None,
+        port: int = None,
         **kwargs
     ):
         super(PGCatalog, self).__init__(**kwargs)
         self.user: str = user
         self.password: str = password
         self.host: str = host
-        self.port: int = int(port) if port is not None else 5432
+        self.port: int = port if port is not None else 5432
         self.database: str = database
 
     @property
     def engine(self) -> object:
         if self._engine is None:
             self._engine = create_engine(
                 "postgresql://{user}:{password}@{host}:{port}/{database}".format(
```

### Comparing `dbcat-0.8.3/dbcat/catalog/db.py` & `dbcat-0.9.0/dbcat/catalog/db.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/catalog/models.py` & `dbcat-0.9.0/dbcat/catalog/models.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/catalog/sqlite_extractor.py` & `dbcat-0.9.0/dbcat/catalog/sqlite_extractor.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/migrations/env.py` & `dbcat-0.9.0/dbcat/migrations/env.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/migrations/versions/3509a9f07432_add_athena_columns.py` & `dbcat-0.9.0/dbcat/migrations/versions/3509a9f07432_add_athena_columns.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/migrations/versions/477d6d4b6ad7_add_update_create_columns.py` & `dbcat-0.9.0/dbcat/migrations/versions/477d6d4b6ad7_add_update_create_columns.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/migrations/versions/7d2638f2ab5f_add_tasks_table.py` & `dbcat-0.9.0/dbcat/migrations/versions/7d2638f2ab5f_add_tasks_table.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/migrations/versions/d1daff1715f7_initial_run.py` & `dbcat-0.9.0/dbcat/migrations/versions/d1daff1715f7_initial_run.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/dbcat/migrations/versions/d2c711b84996_add_pii_type_enum_to_column.py` & `dbcat-0.9.0/dbcat/migrations/versions/d2c711b84996_add_pii_type_enum_to_column.py`

 * *Files identical despite different names*

### Comparing `dbcat-0.8.3/pyproject.toml` & `dbcat-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbcat"
-version = "0.8.3"
+version = "0.9.0"
 description = "Tokern Data Catalog"
 authors = ["Tokern <info@tokern.io>"]
 license = "MIT"
 classifiers = [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
@@ -33,26 +33,27 @@
 pyhocon = "^0.3.58"
 pyathena = {version = "1.11.5", extras = ["sqlalchemy"]}
 PyMySQL = "^1.0.2"
 SQLAlchemy = "~=1.3.24"
 botocore = "~=1.20.23"
 pyparsing = "~=2.0"
 boto3 = "1.17.23"
+typer = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "==19.10b0"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pre-commit = "*"
 pytest = "*"
 pytest-cov = "*"
 types-PyYAML = "^5.4.3"
 types-PyMySQL = "^1.0.0"
-pytest-lazy-fixture = "^0.6.3"
+pytest-cases = "^3.6.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-dbcat = "dbcat.__main__:main"
+dbcat = "dbcat.__main__:app"
```

### Comparing `dbcat-0.8.3/setup.py` & `dbcat-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,23 @@
  'botocore>=1.20.23,<1.21.0',
  'click',
  'psycopg2>=2.9.1,<3.0.0',
  'pyathena[sqlalchemy]==1.11.5',
  'pyhocon>=0.3.58,<0.4.0',
  'pyparsing>=2.0,<3.0',
  'snowflake-sqlalchemy==1.2.4',
- 'sqlalchemy-mixins>=1.5,<2.0']
+ 'sqlalchemy-mixins>=1.5,<2.0',
+ 'typer>=0.4.0,<0.5.0']
 
 entry_points = \
-{'console_scripts': ['dbcat = dbcat.__main__:main']}
+{'console_scripts': ['dbcat = dbcat.__main__:app']}
 
 setup_kwargs = {
     'name': 'dbcat',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'Tokern Data Catalog',
     'long_description': '[![CircleCI](https://circleci.com/gh/tokern/dbcat.svg?style=svg)](https://circleci.com/gh/tokern/dbcat)\n[![codecov](https://codecov.io/gh/tokern/dbcat/branch/main/graph/badge.svg)](https://codecov.io/gh/tokern/dbcat)\n[![PyPI](https://img.shields.io/pypi/v/dbcat.svg)](https://pypi.python.org/pypi/dbcat)\n[![image](https://img.shields.io/pypi/l/dbcat.svg)](https://pypi.org/project/dbcat/)\n[![image](https://img.shields.io/pypi/pyversions/dbcat.svg)](https://pypi.org/project/dbcat/)\n\n# Data Catalog for Databases and Data Warehouses\n\n## Overview\n\n*dbcat* builds and maintains metadata from all your databases and data warehouses. \n*dbcat* is simple to use and maintain. Build a data catalog in minutes by providing\ncredentials using a command line application or API. Automate collection of metadata using\ncron or other workflow automation tools.\n\n*dbcat* stores the catalog in a Postgresql database. Use cloud hosting platforms to ease \noperations in maintaining the catalog in a Postgresql database. \n\nAccess the catalog using raw sql or the python APIs provided by *dbcat* in your python\napplication.\n\n## Quick Start\n\n*dbcat* is distributed as a python application.\n\n    python3 -m venv .env\n    source .env/bin/activate\n    pip install piicatcher\n\n    # configure the application\n    \n    dbcat -c <config dir> pull\n\n## Supported Technologies\n\nThe following databases are supported:\n\n* MySQL/Mariadb\n* PostgreSQL\n* AWS Redshift\n* BigQuery\n* Snowflake\n* AWS Glue\n\n',
     'author': 'Tokern',
     'author_email': 'info@tokern.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://tokern.io/',
```

### Comparing `dbcat-0.8.3/PKG-INFO` & `dbcat-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbcat
-Version: 0.8.3
+Version: 0.9.0
 Summary: Tokern Data Catalog
 Home-page: https://tokern.io/
 License: MIT
 Keywords: data-catalog,postgres,snowflake,redshift,glue
 Author: Tokern
 Author-email: info@tokern.io
 Requires-Python: >=3.8,<4.0
@@ -28,14 +28,15 @@
 Requires-Dist: click
 Requires-Dist: psycopg2 (>=2.9.1,<3.0.0)
 Requires-Dist: pyathena[sqlalchemy] (==1.11.5)
 Requires-Dist: pyhocon (>=0.3.58,<0.4.0)
 Requires-Dist: pyparsing (>=2.0,<3.0)
 Requires-Dist: snowflake-sqlalchemy (==1.2.4)
 Requires-Dist: sqlalchemy-mixins (>=1.5,<2.0)
+Requires-Dist: typer (>=0.4.0,<0.5.0)
 Project-URL: Repository, https://github.com/tokern/dbcat/
 Description-Content-Type: text/markdown
 
 [![CircleCI](https://circleci.com/gh/tokern/dbcat.svg?style=svg)](https://circleci.com/gh/tokern/dbcat)
 [![codecov](https://codecov.io/gh/tokern/dbcat/branch/main/graph/badge.svg)](https://codecov.io/gh/tokern/dbcat)
 [![PyPI](https://img.shields.io/pypi/v/dbcat.svg)](https://pypi.python.org/pypi/dbcat)
 [![image](https://img.shields.io/pypi/l/dbcat.svg)](https://pypi.org/project/dbcat/)
```

