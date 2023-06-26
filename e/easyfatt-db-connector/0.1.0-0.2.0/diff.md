# Comparing `tmp/easyfatt_db_connector-0.1.0.tar.gz` & `tmp/easyfatt_db_connector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfatt_db_connector-0.1.0.tar", max compression
+gzip compressed data, was "easyfatt_db_connector-0.2.0.tar", max compression
```

## Comparing `easyfatt_db_connector-0.1.0.tar` & `easyfatt_db_connector-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.1.0/LICENSE
--rw-r--r--   0        0        0      676 2023-05-13 23:14:06.516585 easyfatt_db_connector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2023-05-05 16:25:07.423683 easyfatt_db_connector-0.1.0/README.md
--rw-r--r--   0        0        0       68 2023-05-05 17:04:51.361083 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/__init__.py
--rw-r--r--   0        0        0      253 2023-05-05 17:04:51.387584 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/constants.py
--rw-r--r--   0        0        0       52 2023-05-05 17:04:51.377081 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/core/__init__.py
--rw-r--r--   0        0        0      294 2023-05-05 17:04:51.438081 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/core/exceptions.py
--rw-r--r--   0        0        0     4387 2023-05-13 23:14:16.161300 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/core/methods/fdb.py
--rw-r--r--   0        0        0     4701 2023-05-14 00:56:19.976885 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/core/methods/sqlalchemy.py
--rw-r--r--   0        0        0     3239 2023-05-13 23:14:36.338990 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/downloader.py
--rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/__init__.py
--rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/dynamic/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/dynamic/factory.py
--rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/static/__init__.py
--rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/static/models.py
--rw-r--r--   0        0        0      931 2023-05-14 00:24:15.812388 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/test.py
--rw-r--r--   0        0        0      206 2023-05-07 21:46:46.281803 easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/utils.py
--rw-r--r--   0        0        0     2842 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.2.0/LICENSE
+-rw-r--r--   0        0        0      676 2023-06-26 18:42:19.602373 easyfatt_db_connector-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2023-06-26 18:42:58.676372 easyfatt_db_connector-0.2.0/README.md
+-rw-r--r--   0        0        0       68 2023-05-05 17:04:51.361083 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/__init__.py
+-rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/constants.py
+-rw-r--r--   0        0        0       52 2023-05-05 17:04:51.377081 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/__init__.py
+-rw-r--r--   0        0        0     6904 2023-06-26 18:40:35.472374 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_base.py
+-rw-r--r--   0        0        0     2974 2023-06-26 18:40:35.472374 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_fdb.py
+-rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
+-rw-r--r--   0        0        0      294 2023-05-05 17:04:51.438081 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/exceptions.py
+-rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/dynamic/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/dynamic/factory.py
+-rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/static/__init__.py
+-rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/static/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/decorators.py
+-rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/downloader.py
+-rw-r--r--   0        0        0     2842 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.2.0/PKG-INFO
```

### Comparing `easyfatt_db_connector-0.1.0/LICENSE` & `easyfatt_db_connector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.1.0/pyproject.toml` & `easyfatt_db_connector-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "easyfatt-db-connector"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Luca Salvarani <lucasalvarani99@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "easyfatt_db_connector", from = "./src/"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 requests = "^2.30.0"
 fdb = "^2.0.2"
-sqlalchemy-firebird = "^0.8.0"
+sqlalchemy-firebird = "^2.0.0"
 sqlalchemy = "^2.0.12"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 poethepoet = "^0.20.0"
```

### Comparing `easyfatt_db_connector-0.1.0/README.md` & `easyfatt_db_connector-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/core/methods/fdb.py` & `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
-from typing import Any, Literal, Optional
+from contextlib import contextmanager
+import time
 
 from pathlib import Path
 import shutil
 
-import fdb
-from fdb.fbcore import _RowMapping
 from fdb.ibase import charset_map
 
+import sqlalchemy
+# import sqlalchemy_firebird
+
 from easyfatt_db_connector.core.exceptions import FirebirdClientError
 from easyfatt_db_connector.constants import (
     DEFAULT_DATABASE_CHARSET,
     DEFAULT_DATABASE_PASSWORD,
     DEFAULT_DATABASE_USERNAME,
     DEFAULT_FIREBIRD_LOCATION,
 )
 
 
 class EasyfattDB(object):
+    """ Implementation of the `EasyfattDBGeneric` class using the `sqlalchemy` library. """
     archive_path: Path
     firebird_path: Path
 
     db_username: str
     db_password: str
     db_charset: str | None
 
@@ -40,76 +43,99 @@
             firebird_path (Path, optional): The Firebird Embedded installation path
             db_user (str, optional): The user that will be used to connect to the database.
             db_password (str, optional): The password that will be used to connect to the database.
             db_charset (str | None, optional): The character set that will be used to interpret data.
         """
         self.archive_path = Path(archive_path).expanduser().resolve()
         self.firebird_path = Path(firebird_path).expanduser().resolve()
-
-        if db_charset not in charset_map.keys():
+        
+        if db_charset is None:
+            self.db_charset = charset_map[None]
+
+        elif db_charset.upper() in charset_map.keys():
+            self.db_charset = charset_map[db_charset]
+            
+        elif db_charset in charset_map.values():
+            self.db_charset = db_charset
+        else:
             supported_charsets = ", ".join([str(charset) for charset in charset_map.keys()])
 
             raise FirebirdClientError(
                 f"Character set '{db_charset}' not valid. Use one of '{supported_charsets}'"
             )
 
         self.db_username = db_user
         self.db_password = db_password
-        self.db_charset = db_charset
 
         # Check if Firebase Embedded is installed
         if not self.firebird_path.exists():
             raise FirebirdClientError(f"The path '{self.firebird_path}' does not exist.")
 
         if not (self.firebird_path / "fbembed.dll").exists():
             raise FirebirdClientError(
                 f"The path '{self.firebird_path}' MUST contain the file 'fbembed.dll'."
             )
 
-        # Questa riga è fondamentale!
-        # Stiamo dicendo a fdb dove si trovano i binari di Firebird Embedded (vedi https://stackoverflow.com/a/62245011/8965861)!
-        fdb.load_api(str(self.firebird_path / "fbembed.dll"))
 
-    def _connect(self):
-        try:
-            # Use `WIN1252` instead of `UTF8` to fix error "SQLCODE: -204 block size exceeds implementation restriction"
-            # See https://stackoverflow.com/q/40170882/8965861
-            print(f"Connecting to database '{self.archive_path}'")
-            fdb.connect(
-                database=str(self.archive_path),
-                user=self.db_username,
-                # password=self.db_password,
-                charset=self.db_charset,
-            )
-        except (fdb.DatabaseError, UnicodeDecodeError) as e:
-            if "codec can't decode byte" in str(e) or "lock manager" in str(e):
-                return True
-            else:
-                raise
-        else:
-            return False
+    def create_engine(self, username=None, password=None, database_path: Path=None):
+        connection_url = sqlalchemy.URL.create(
+            drivername="firebird",
+            username=self.db_username if username is None else username,
+            database=str(self.archive_path.resolve() if database_path is None else database_path.resolve()),
+            query={
+                "fb_library_name": str(self.firebird_path / "fbembed.dll"),
+                "charset": self.db_charset,
+                # "user": self.db_username if username is None else username
+            }
+        )
+        return sqlalchemy.create_engine(connection_url, echo=False)
+    
+    @contextmanager
+    def connect(self, engine: sqlalchemy.engine.base.Engine = None):
+        """Connect to the database and return a connection object.
+
+        Can be used as a context manager.
+
+        Args:
+            engine (sqlalchemy.engine.base.Engine, optional): The engine that will be used to connect to the database. Defaults to None.
+
+        Yields:
+            sqlalchemy.engine.base.Connection: The connection object.
+        """
+        temp_database = None
+
+        if engine is None:
+            temp_database = Path(f"{self.archive_path}.tmp~")
+            shutil.copy(self.archive_path, temp_database)
+    
+            engine = self.create_engine(database_path=temp_database)
 
-    def is_locked(self):
         try:
-            # Use `WIN1252` instead of `UTF8` to fix error "SQLCODE: -204 block size exceeds implementation restriction"
-            # See https://stackoverflow.com/q/40170882/8965861
-            print(f"Connecting to database '{self.archive_path}'")
-            fdb.connect(
-                database=str(self.archive_path),
-                user=self.db_username,
-                # password=self.db_password,
-                charset=self.db_charset,
-            )
-        except (fdb.DatabaseError, UnicodeDecodeError) as e:
-            if "codec can't decode byte" in str(e) or "lock manager" in str(e):
-                return True
+            with engine.connect() as connection:
+                yield connection
+
+            if temp_database is not None:
+                engine.dispose()
+            
+        except sqlalchemy.exc.OperationalError as e:
+            if "lock manager" in str(e):
+                raise FirebirdClientError(
+                    f"The database '{self.archive_path}' is locked. Close Easyfatt and try again."
+                )
             else:
                 raise
-        else:
-            return False
+        finally:
+            if temp_database is not None:
+                try:
+                    engine.dispose()
+                except:
+                    pass
+                temp_database.unlink(missing_ok=True)
+
 
 
 if __name__ == "__main__":
+    print("Start")
     database_path = Path("~/Documents/Danea Easyfatt/TestArchivio.eft").expanduser()
 
     db = EasyfattDB(database_path)
-    print(f"- Is database locked? {db.is_locked()}")
+    print(f"- Engine: {db.create_engine()}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/downloader.py` & `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/downloader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from __future__ import annotations
 
 import sys
+import logging
 from typing import Literal
 
 from pathlib import Path
 import shutil
 
 from urllib.parse import urlparse
 import requests
 
 from easyfatt_db_connector.constants import DEFAULT_FIREBIRD_LOCATION
 
 RELEASE_URL = "https://api.github.com/repos/FirebirdSQL/firebird/releases"
 PROCESSOR_ARCHITECTURE = 32 << bool(sys.maxsize >> 32)
 
+logger = logging.getLogger(__name__)
+
+__all__ = ["get_available_releases", "download"]
 
 def get_available_releases() -> list[str]:
+    """ Retrieves the available releases from the FirebirdSQL repository.
+
+    Returns:
+        releases (list[str]): List of available release tags.
+    """
     response = requests.get(RELEASE_URL)
 
     return [
         release["tag_name"]
         for release in response.json()
         if list(
             filter(
-                lambda a: "_x64_embed.zip" in a["name"] or "_Win32_embed.zip" in a["name"],
+                lambda a: "_x64_embed.zip" in a["name"]
+                or "_Win32_embed.zip" in a["name"],
                 release["assets"],
             )
         )
     ]
 
 
 def download(
@@ -39,59 +49,81 @@
 
     Args:
         tag_name ('R2_5_8' | 'R2_5_9', optional): The tag name of the release (see https://github.com/FirebirdSQL/firebird/releases).
         firebird_path (Path, optional): Path where the firebird database will be installed. Defaults to `~/.cache/firebird-embedded/`.
         architecture (Literal[32, 64] | None, optional): Desired processor architecture (32 or 64 bit, None for automatic discovery). Defaults to None.
 
     Raises:
-        Exception: _description_
+        Exception: No available releases were found
+        Exception: Release '{tag_name}' not found. Available releases are {available_releases}.
+        Exception: Unexpected number of downloads found: {download_no}. Expected 1.
 
     Returns:
         firebird (Path): Path to the Firebase Embedded folder
     """
-    release_name = tag_name if tag_name is not None else get_available_releases()[0]
+    available_releases = get_available_releases()
+
+    desired_architecture = (
+        architecture if architecture is not None else PROCESSOR_ARCHITECTURE
+    )
+
+    if len(available_releases) == 0:
+        raise Exception("No available releases were found")
+    elif tag_name is not None and tag_name not in available_releases:
+        raise Exception(f"Release '{tag_name}' not found. Available releases are {', '.join(available_releases)}.")
+
+    release_name = tag_name if tag_name is not None else available_releases[0]
     release = requests.get(
         f"https://api.github.com/repos/FirebirdSQL/firebird/releases/tags/{release_name}"
     ).json()
     assets = release["assets"]
 
-    desired_architecture = architecture if architecture is not None else PROCESSOR_ARCHITECTURE
-
+    # Retrieve the download url for the desired architecture
     remote_package_urls = [
         asset["browser_download_url"]
         for asset in assets
-        if ("_x64_embed.zip" if desired_architecture == 64 else "_Win32_embed.zip") in asset["name"]
+        if ("_x64_embed.zip" if desired_architecture == 64 else "_Win32_embed.zip")
+        in asset["name"]
     ]
 
     if len(remote_package_urls) != 1:
-        raise Exception(f"Unexpected number of downloads found: {', '.join(remote_package_urls)}")
+        raise Exception(
+            f"Unexpected number of downloads found: {', '.join(remote_package_urls)}. Expected 1."
+        )
 
-    # Download and save the zip file
-    zip_file_path: Path = firebird_path / str(urlparse(remote_package_urls[0]).path).split("/")[-1]
+    zip_file_path: Path = (
+        firebird_path / str(urlparse(remote_package_urls[0]).path).split("/")[-1]
+    )
     version_file = firebird_path / "version.txt"
 
-    if version_file.exists() and version_file.read_text() == zip_file_path.stem:
-        return firebird_path
-
-    # Remove all old files
-    for child in firebird_path.glob("*"):
-        if child.is_dir():
-            shutil.rmtree(child)
-        else:
-            child.unlink()
+    try:
+        firebird_path.mkdir(parents=True)
+    except FileExistsError:
+        # Check if version is the same
+        if version_file.exists() and version_file.read_text() == zip_file_path.stem:
+            return firebird_path
+
+        # Remove all old files
+        for child in firebird_path.glob("*"):
+            if child.is_dir():
+                shutil.rmtree(child)
+            else:
+                child.unlink()
 
+    # Download the archive and extract it
     response = requests.get(remote_package_urls[0], allow_redirects=True)
     with open(zip_file_path, "wb") as zip_file:
         zip_file.write(response.content)
 
     shutil.unpack_archive(zip_file_path, firebird_path)
     zip_file_path.unlink()
 
+    # Write the version file
     version_file.write_text(zip_file_path.stem)
 
     return firebird_path
 
 
 if __name__ == "__main__":
     print(download())
-    print(download("R2_5_8"))
+    # print(download("R2_5_8"))
     # print(download("R2_5_9", architecture=32))
```

### Comparing `easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/dynamic/factory.py` & `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/dynamic/factory.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.1.0/src/easyfatt_db_connector/orm/static/models.py` & `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/static/models.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.1.0/PKG-INFO` & `easyfatt_db_connector-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easyfatt-db-connector
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Luca Salvarani
 Author-email: lucasalvarani99@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fdb (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.12,<3.0.0)
-Requires-Dist: sqlalchemy-firebird (>=0.8.0,<0.9.0)
+Requires-Dist: sqlalchemy-firebird (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # easyfatt-db-connector
 
 ## Development
 
 ### Python
```

