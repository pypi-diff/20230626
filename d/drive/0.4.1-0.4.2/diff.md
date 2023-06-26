# Comparing `tmp/drive-0.4.1.tar.gz` & `tmp/drive-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive-0.4.1.tar", max compression
+gzip compressed data, was "drive-0.4.2.tar", max compression
```

## Comparing `drive-0.4.1.tar` & `drive-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-15 10:18:02.983487 drive-0.4.1/LICENSE
--rw-r--r--   0        0        0     4045 2023-05-15 10:18:02.983487 drive-0.4.1/README.md
--rw-r--r--   0        0        0      128 2023-05-15 10:18:02.983487 drive-0.4.1/drive/__init__.py
--rw-r--r--   0        0        0     1178 2023-05-15 10:18:02.983487 drive-0.4.1/drive/auth.py
--rw-r--r--   0        0        0    17494 2023-05-15 10:18:02.983487 drive-0.4.1/drive/client.py
--rw-r--r--   0        0        0      124 2023-05-15 10:18:02.983487 drive-0.4.1/drive/exceptions.py
--rw-r--r--   0        0        0     9562 2023-05-15 10:18:02.983487 drive-0.4.1/drive/files.py
--rw-r--r--   0        0        0     1076 2023-05-15 10:18:02.983487 drive-0.4.1/drive/mimetypes.py
--rw-r--r--   0        0        0        0 2023-05-15 10:18:02.983487 drive-0.4.1/drive/py.typed
--rw-r--r--   0        0        0     1053 2023-05-15 10:18:02.983487 drive-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 drive-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-26 14:40:38.276769 drive-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4045 2023-06-26 14:40:38.276769 drive-0.4.2/README.md
+-rw-r--r--   0        0        0      128 2023-06-26 14:40:38.276769 drive-0.4.2/drive/__init__.py
+-rw-r--r--   0        0        0     1363 2023-06-26 14:40:38.276769 drive-0.4.2/drive/auth.py
+-rw-r--r--   0        0        0    17433 2023-06-26 14:40:38.276769 drive-0.4.2/drive/client.py
+-rw-r--r--   0        0        0      124 2023-06-26 14:40:38.276769 drive-0.4.2/drive/exceptions.py
+-rw-r--r--   0        0        0     9546 2023-06-26 14:40:38.276769 drive-0.4.2/drive/files.py
+-rw-r--r--   0        0        0     1076 2023-06-26 14:40:38.276769 drive-0.4.2/drive/mimetypes.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:40:38.276769 drive-0.4.2/drive/py.typed
+-rw-r--r--   0        0        0     1459 2023-06-26 14:40:38.276769 drive-0.4.2/drive/sheets.py
+-rw-r--r--   0        0        0     1111 2023-06-26 14:40:38.276769 drive-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 drive-0.4.2/PKG-INFO
```

### Comparing `drive-0.4.1/LICENSE` & `drive-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drive-0.4.1/README.md` & `drive-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `drive-0.4.1/drive/auth.py` & `drive-0.4.2/drive/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # -*- coding: UTF-8 -*-
 
 import os
-import httplib2  # type: ignore
+import httplib2
 from os import environ
 from typing import Optional
 
 from oauth2client.service_account import ServiceAccountCredentials  # type: ignore
 
 from drive.exceptions import DriveException
 
 ENV_CLIENT_SECRET_PATH = "GOOGLE_APPLICATION_CREDENTIALS"
 
-# If you modify these scopes, delete your previously saved credentials
+# If you modify these scopes, delete your previously-saved credentials
 DRIVE_SCOPE = 'https://www.googleapis.com/auth/drive'
 
 
 class MissingCredentialsException(DriveException):
     def __init__(self):
         super().__init__("Missing credentials! Please set %s" % ENV_CLIENT_SECRET_PATH)
 
 
 def get_credentials(path: Optional[str] = None):
     """
     Retrieve the user's Google Cloud credentials.
-    :param path:
-    :return:
     """
 
     if path is None:
-        path = environ["GOOGLE_APPLICATION_CREDENTIALS"]
+        if ENV_CLIENT_SECRET_PATH not in environ:
+            raise MissingCredentialsException()
+
+        path = environ[ENV_CLIENT_SECRET_PATH]
 
     path = os.path.expanduser(path)
     creds = ServiceAccountCredentials.from_json_keyfile_name(path, scopes=[DRIVE_SCOPE])
     if not creds or creds.invalid:
         raise MissingCredentialsException()
     return creds
 
 
 def authorize(credentials):
-    """
-    :param credentials:
-    :return:
-    """
     return credentials.authorize(httplib2.Http())
+
+
+def authorize_credentials(credentials_path: Optional[str] = None):
+    """Equivalent of authorize(get_credentials(credentials_path))."""
+    return authorize(get_credentials(credentials_path))
```

### Comparing `drive-0.4.1/drive/client.py` & `drive-0.4.2/drive/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import io
 import os.path
 import random
 import sys
 import time
 from typing import Optional, List, Any, Tuple, Dict, cast, Iterable, Union
 
-import httplib2  # type: ignore
-import openpyxl  # type: ignore
+import httplib2
+import openpyxl
 from apiclient import discovery  # type: ignore
 from googleapiclient.errors import HttpError  # type: ignore
 from googleapiclient.http import MediaIoBaseDownload, MediaIoBaseUpload  # type: ignore
 
 from drive import mimetypes
-from drive.auth import authorize, get_credentials
+from drive.auth import authorize_credentials
 from drive.exceptions import FileNotFoundException
 from drive.files import File, guess_original_mime_type
 
 # Retry transport and file IO errors.
 RETRYABLE_ERRORS = (httplib2.HttpLib2Error, IOError)
 # Default number of bytes to send/receive in each request.
 CHUNKSIZE = 2 * 1024 * 1024
@@ -28,14 +28,15 @@
 
 def handle_progressless_iter(error, progressless_iters, *, retries_count=5):
     if progressless_iters > retries_count:
         print('Failed to make progress for too many consecutive iterations.')
         raise error
 
     sleep_time = random.random() * (2 ** progressless_iters)
+    # TODO: use a logger
     print('Caught exception (%s). Sleeping for %s seconds before retry #%d.'
           % (str(error), sleep_time, progressless_iters))
     time.sleep(sleep_time)
 
 
 def print_with_carriage_return(s):
     """
@@ -85,21 +86,18 @@
     if isinstance(value, bool):
         return "true" if value else "false"
 
     return "'%s'" % str(value).replace("\\", "\\\\").replace("'", "\\'")
 
 
 class Client:
-    """
-    Google Drive client
-    """
+    """Google Drive client"""
 
     def __init__(self, credentials_path: Optional[str] = None, *, download_retries_count=5):
-        credentials = get_credentials(credentials_path)
-        http = authorize(credentials)
+        http = authorize_credentials(credentials_path)
         self.service = discovery.build('drive', 'v3', http=http)
         self.download_retries_count = download_retries_count
 
     @property
     def _files(self):
         return self.service.files()
```

### Comparing `drive-0.4.1/drive/files.py` & `drive-0.4.2/drive/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 
 import io
 import json
 from typing import Optional, Union, cast, Dict, Any, BinaryIO
 
-from openpyxl.workbook import Workbook  # type: ignore
+from openpyxl.workbook import Workbook
 
 import drive
 from drive import mimetypes
 
 
 class File:
     """
```

### Comparing `drive-0.4.1/drive/mimetypes.py` & `drive-0.4.2/drive/mimetypes.py`

 * *Files identical despite different names*

### Comparing `drive-0.4.1/pyproject.toml` & `drive-0.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drive"
-version = "0.4.1"
+version = "0.4.2"
 description = "Google Drive client"
 authors = ["Baptiste Fontaine <b@ptistefontaine.fr>"]
 license = "MIT"
 include = ["drive/py.typed"]
 readme = "README.md"
 packages = [
     { include = "drive" },
@@ -26,14 +26,16 @@
 python-magic = "^0.4.27"
 python-magic-bin = {version = "^0.4.14", platform = "windows"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 mypy = "^0"
+types-openpyxl = "^3.1.0.13"
+types-httplib2 = "^0.22.0.1"
 
 [tool.coverage.report]
 omit = ["tests/*"]
 exclude_lines = [
     "pragma: nocover",
     "raise NotImplementedError",
     "except ImportError:",
```

### Comparing `drive-0.4.1/PKG-INFO` & `drive-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: drive
-Version: 0.4.1
+Version: 0.4.2
 Summary: Google Drive client
 License: MIT
 Author: Baptiste Fontaine
 Author-email: b@ptistefontaine.fr
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: google-api-python-client (>=2.64.0,<3.0.0)
 Requires-Dist: httplib2 (>=0.20.4,<0.21.0)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "windows"
 Description-Content-Type: text/markdown
```

