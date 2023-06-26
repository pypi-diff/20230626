# Comparing `tmp/gundi_client-1.0.0.tar.gz` & `tmp/gundi_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_client-1.0.0.tar", max compression
+gzip compressed data, was "gundi_client-1.0.1.tar", max compression
```

## Comparing `gundi_client-1.0.0.tar` & `gundi_client-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,6 @@
--rw-r--r--   0        0        0     1681 2023-06-06 07:27:28.357433 gundi_client-1.0.0/README.md
--rw-r--r--   0        0        0      358 2023-05-09 15:53:31.705675 gundi_client-1.0.0/gundi_client/.env.local
--rw-r--r--   0        0        0       30 2023-05-24 04:47:28.211754 gundi_client-1.0.0/gundi_client/__init__.py
--rw-r--r--   0        0        0     9887 2023-06-06 07:27:28.358366 gundi_client-1.0.0/gundi_client/client.py
--rw-r--r--   0        0        0    13842 2023-05-24 04:47:28.212310 gundi_client-1.0.0/gundi_client/schemas.py
--rw-r--r--   0        0        0      890 2023-05-24 04:47:28.212516 gundi_client-1.0.0/gundi_client/settings.py
--rw-r--r--   0        0        0      560 2023-05-24 06:06:40.882965 gundi_client-1.0.0/gundi_client/test.py
--rw-r--r--   0        0        0      767 2023-06-06 07:27:28.359914 gundi_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 gundi_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1681 2023-06-16 14:08:58.192263 gundi_client-1.0.1/README.md
+-rw-r--r--   0        0        0       30 2023-06-16 14:08:58.192263 gundi_client-1.0.1/gundi_client/__init__.py
+-rw-r--r--   0        0        0     9897 2023-06-16 14:08:58.192263 gundi_client-1.0.1/gundi_client/client.py
+-rw-r--r--   0        0        0      890 2023-06-16 14:08:58.192263 gundi_client-1.0.1/gundi_client/settings.py
+-rw-r--r--   0        0        0      789 2023-06-26 16:12:24.603826 gundi_client-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 gundi_client-1.0.1/PKG-INFO
```

### Comparing `gundi_client-1.0.0/README.md` & `gundi_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gundi_client-1.0.0/gundi_client/client.py` & `gundi_client-1.0.1/gundi_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from datetime import datetime, timedelta, timezone
 from typing import List, Dict, Any
 from uuid import UUID
 from pydantic import parse_obj_as
 from . import settings
-from .schemas import (
+from gundi_core.schemas import (
     IntegrationInformation,
     OAuthToken,
     TIntegrationInformation,
     DeviceState,
     OutboundConfiguration,
 )
 from httpx import (
```

### Comparing `gundi_client-1.0.0/gundi_client/settings.py` & `gundi_client-1.0.1/gundi_client/settings.py`

 * *Files identical despite different names*

### Comparing `gundi_client-1.0.0/pyproject.toml` & `gundi_client-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gundi-client"
-version = "1.0.0"
+version = "1.0.1"
 description = "An async client for Gundi's API"
 authors = [
     "Rohit Chaudhri <rohitc@vulcan.com>",
     "Matt Morrissette <matt.morrissette@wildlifeprotectionsolutions.org>",
     "Chris Doehring <chrisdo@earthranger.com>",
     "Mariano M <marianom@earthranger.com>",
     "Victor Garcia <victorg@earthranger.com>"
@@ -18,14 +18,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 environs = "^9.5"
 pydantic = "^1.10"
 httpx = "^0.24.0"
 respx = "^0.20.1"
+gundi-core = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 
 [build-system]
```

### Comparing `gundi_client-1.0.0/PKG-INFO` & `gundi_client-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gundi-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: An async client for Gundi's API
 License: Apache-2.0
 Author: Rohit Chaudhri
 Author-email: rohitc@vulcan.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: environs (>=9.5,<10.0)
+Requires-Dist: gundi-core (>=1.0.0,<2.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: respx (>=0.20.1,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Gundi Client
 ## Introduction
```

