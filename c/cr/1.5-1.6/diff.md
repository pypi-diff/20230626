# Comparing `tmp/cr-1.5.tar.gz` & `tmp/cr-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cr-1.5.tar", last modified: Fri Nov  4 22:35:46 2022, max compression
+gzip compressed data, was "cr-1.6.tar", last modified: Mon Jun 26 01:43:59 2023, max compression
```

## Comparing `cr-1.5.tar` & `cr-1.6.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-11-04 22:35:46.220077 cr-1.5/
--rw-rw-rw-   0        0        0     1068 2022-09-27 16:03:02.000000 cr-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     2062 2022-11-04 22:35:46.220077 cr-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      341 2022-09-29 20:38:06.000000 cr-1.5/README.md
-drwxrwxrwx   0        0        0        0 2022-11-04 22:35:46.093128 cr-1.5/cr/
--rw-rw-rw-   0        0        0      914 2022-10-30 03:03:28.000000 cr-1.5/cr/__init__.py
--rw-rw-rw-   0        0        0    16472 2022-10-28 00:52:42.000000 cr-1.5/cr/api.py
--rw-rw-rw-   0        0        0    20205 2022-10-28 00:52:42.000000 cr-1.5/cr/cli.py
--rw-rw-rw-   0        0        0     3157 2022-10-07 03:16:52.000000 cr-1.5/cr/config.py
--rw-rw-rw-   0        0        0    13074 2022-10-28 00:52:42.000000 cr-1.5/cr/rich_utils.py
--rw-rw-rw-   0        0        0     7929 2022-10-19 19:12:29.000000 cr-1.5/cr/ssh.py
-drwxrwxrwx   0        0        0        0 2022-11-04 22:35:46.220077 cr-1.5/cr/templates/
--rw-rw-rw-   0        0        0      338 2022-10-28 00:52:42.000000 cr-1.5/cr/templates/settings-mariadb.py.txt
--rw-rw-rw-   0        0        0      306 2022-10-28 00:52:42.000000 cr-1.5/cr/templates/settings-postgres.py.txt
--rw-rw-rw-   0        0        0      141 2022-10-28 00:52:42.000000 cr-1.5/cr/templates/settings-sqlite.py.txt
--rw-rw-rw-   0        0        0      119 2022-10-28 00:52:42.000000 cr-1.5/cr/templates/settings-top.py.txt
--rw-rw-rw-   0        0        0       63 2022-10-28 00:52:42.000000 cr-1.5/cr/templates/settings-wagtail.py.txt
--rw-rw-rw-   0        0        0      480 2022-10-28 00:52:42.000000 cr-1.5/cr/templates/settings.py.txt
--rw-rw-rw-   0        0        0    12792 2022-11-02 03:51:57.000000 cr-1.5/cr/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-04 22:35:46.141773 cr-1.5/cr.egg-info/
--rw-rw-rw-   0        0        0     2062 2022-11-04 22:35:45.000000 cr-1.5/cr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2022-11-04 22:35:46.000000 cr-1.5/cr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-04 22:35:45.000000 cr-1.5/cr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2022-11-04 22:35:45.000000 cr-1.5/cr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2022-11-04 22:35:45.000000 cr-1.5/cr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2022-11-04 22:35:45.000000 cr-1.5/cr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1145 2022-10-28 00:53:06.000000 cr-1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-04 22:35:46.220077 cr-1.5/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 01:43:59.946586 cr-1.6/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1068 2023-06-26 01:42:58.000000 cr-1.6/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-06-26 01:43:59.946586 cr-1.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      341 2023-06-26 01:42:58.000000 cr-1.6/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 01:43:59.942586 cr-1.6/cr/
+-rw-r--r--   0 vsts      (1001) docker     (122)      934 2023-06-26 01:42:58.000000 cr-1.6/cr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16977 2023-06-26 01:42:58.000000 cr-1.6/cr/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20879 2023-06-26 01:42:58.000000 cr-1.6/cr/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3214 2023-06-26 01:42:58.000000 cr-1.6/cr/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13566 2023-06-26 01:42:58.000000 cr-1.6/cr/rich_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8013 2023-06-26 01:42:58.000000 cr-1.6/cr/ssh.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 01:43:59.946586 cr-1.6/cr/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      338 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings-mariadb.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      338 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings-mysql.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings-postgres.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      141 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings-sqlite.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings-top.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings-wagtail.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-06-26 01:42:58.000000 cr-1.6/cr/templates/settings.py.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    13537 2023-06-26 01:42:58.000000 cr-1.6/cr/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 01:43:59.946586 cr-1.6/cr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-06-26 01:43:59.000000 cr-1.6/cr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      585 2023-06-26 01:43:59.000000 cr-1.6/cr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-26 01:43:59.000000 cr-1.6/cr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       35 2023-06-26 01:43:59.000000 cr-1.6/cr.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-06-26 01:43:59.000000 cr-1.6/cr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        3 2023-06-26 01:43:59.000000 cr-1.6/cr.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1338 2023-06-26 01:42:58.000000 cr-1.6/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-06-26 01:43:59.946586 cr-1.6/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 01:43:59.946586 cr-1.6/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)      298 2023-06-26 01:42:58.000000 cr-1.6/tests/test_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3163 2023-06-26 01:42:58.000000 cr-1.6/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2216 2023-06-26 01:42:58.000000 cr-1.6/tests/test_utils.py
```

### Comparing `cr-1.5/LICENSE.txt` & `cr-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cr-1.5/PKG-INFO` & `cr-1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: cr
-Version: 1.5
-Summary: The official CodeRed Cloud command line tool.
-Author-email: CodeRed LLC <info@coderedcorp.com>
-License: MIT License
-        
-        Copyright (c) 2022 CodeRed LLC
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://www.codered.cloud/cli/
-Project-URL: Source, https://github.com/coderedcorp/cr
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-`cr` - CodeRed Cloud CLI
-========================
-
-The official CodeRed Cloud command line tool. Easily deploy your Django, Wagtail, WordPress, or Static HTML sites directly from your terminal or version control system.
-
-https://www.codered.cloud/cli/
-
----
-
-To contribute, see the [CONTRIBUTING.md](CONTRIBUTING.md) file in this repository.
+Metadata-Version: 2.1
+Name: cr
+Version: 1.6
+Summary: The official CodeRed Cloud command line tool.
+Author-email: CodeRed LLC <info@coderedcorp.com>
+License: MIT License
+        
+        Copyright (c) 2022 CodeRed LLC
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://www.codered.cloud/cli/
+Project-URL: Source, https://github.com/coderedcorp/cr
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+`cr` - CodeRed Cloud CLI
+========================
+
+The official CodeRed Cloud command line tool. Easily deploy your Django, Wagtail, WordPress, or Static HTML sites directly from your terminal or version control system.
+
+https://www.codered.cloud/cli/
+
+---
+
+To contribute, see the [CONTRIBUTING.md](CONTRIBUTING.md) file in this repository.
```

### Comparing `cr-1.5/cr/__init__.py` & `cr-1.6/cr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import enum
 import logging
 
 
-VERSION = "1.5"
+VERSION = "1.6"
 
 
 DOCS_LINK = "https://www.codered.cloud/cli/"
 
 
 # Logger for this module.
 LOGGER = logging.getLogger("cr")
@@ -40,14 +40,15 @@
 
     def __str__(self):
         return self.value
 
 
 class DatabaseType(enum.Enum):
     MARIADB = "mariadb"
+    MYSQL = "mysql"
     POSTGRES = "postgres"
 
     def __str__(self):
         return self.value
 
 
 class Env(enum.Enum):
```

### Comparing `cr-1.5/cr/api.py` & `cr-1.6/cr/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """
 Utilities to call CodeRed Cloud API.
 
 Copyright (c) 2022 CodeRed LLC.
 """
+import json
+import time
 from http.client import HTTPResponse
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Union
 from urllib.error import HTTPError
-from urllib.request import Request, urlopen
-import json
-import time
+from urllib.request import Request
+from urllib.request import urlopen
 
+import certifi
 from rich.console import Console
-from rich.progress import Progress
 from rich.panel import Panel
-import certifi
+from rich.progress import Progress
 
-from cr import (
-    AppType,
-    ConfigurationError,
-    DOCS_LINK,
-    DatabaseType,
-    Env,
-    LOGGER,
-    USER_AGENT,
-    UserCancelError,
-    VERSION,
-)
-from cr.utils import (
-    django_manage_check,
-    django_requirements_check,
-    django_settings_check,
-    django_settings_fix,
-    django_wsgi_check,
-    django_wsgi_find,
-    html_index_check,
-    wagtail_settings_fix,
-    wordpress_wpconfig_check,
-)
+from cr import AppType
+from cr import ConfigurationError
+from cr import DatabaseType
+from cr import DOCS_LINK
+from cr import Env
+from cr import LOGGER
+from cr import USER_AGENT
+from cr import UserCancelError
+from cr import VERSION
+from cr.utils import django_manage_check
+from cr.utils import django_requirements_check
+from cr.utils import django_settings_check
+from cr.utils import django_settings_fix
+from cr.utils import django_wsgi_check
+from cr.utils import django_wsgi_find
+from cr.utils import html_index_check
+from cr.utils import wagtail_settings_fix
+from cr.utils import wordpress_wpconfig_check
 
 
 class DatabaseServer:
     def __init__(self, hostname: str, db_type: DatabaseType):
         self.hostname: str = hostname
         self.db_type: DatabaseType = db_type
 
@@ -397,16 +399,16 @@
     return d
 
 
 def request_json(
     url: str,
     method: str = "GET",
     headers: Dict[str, str] = {},
-    data: dict = None,
-    timeout: int = None,
+    data: Optional[dict] = None,
+    timeout: Optional[int] = None,
 ) -> Tuple[int, dict]:
     """
     Makes an HTTP request and parses the JSON response.
     """
     # Update headers to request JSON and specify user agent.
     headers["User-Agent"] = USER_AGENT
     if "Accept" not in headers:
@@ -436,32 +438,38 @@
     return (code, d)
 
 
 def coderedapi(
     endpoint: str,
     method: str,
     token: str,
-    data: dict = None,
+    data: Optional[dict] = None,
     ok: List[int] = [200, 201],
 ) -> Tuple[int, Dict[str, Any]]:
     """
     Calls CodeRed Cloud API and returns a tuple of:
     (HTTP status code, dict of returned JSON).
 
     Raises a human-readable exception if the status code is not in ``ok``.
     """
     endpoint = endpoint.lstrip("/")
-    code, d = request_json(
-        f"https://app.codered.cloud/{endpoint}",
-        method=method,
-        headers={
-            "Authorization": f"Token {token}",
-        },
-        data=data,
-    )
+    try:
+        code, d = request_json(
+            f"https://app.codered.cloud/{endpoint}",
+            method=method,
+            headers={
+                "Authorization": f"Token {token}",
+            },
+            data=data,
+        )
+    except Exception:
+        raise Exception(
+            "Error contacting CodeRed API. Please try again shortly."
+        )
+
     # If the code is not within the list of expected status codes, raise an
     # error with the API's error message.
     if ok and code not in ok:
         if "detail" in d:
             raise Exception(d["detail"])
         if "error" in d:
             raise Exception(d["error"])
```

### Comparing `cr-1.5/cr/cli.py` & `cr-1.6/cr/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,44 +18,47 @@
   as a result of an error. This will likely trigger a support case.
 
 Printing output should be done through the CONSOLE object. Print minimal output
 only as necessary for the user to know the program is working.
 
 Copyright (c) 2022 CodeRed LLC.
 """
-from pathlib import Path, PurePosixPath
 import argparse
 import logging
 import sys
+from pathlib import Path
+from pathlib import PurePosixPath
 
 from rich.logging import RichHandler
-from rich.progress import (
-    BarColumn,
-    MofNCompleteColumn,
-    TaskProgressColumn,
-    TimeElapsedColumn,
-    TextColumn,
-)
-from cr import VERSION, DOCS_LINK, LOGGER, UserCancelError
-from cr.api import Env, Webapp, check_update
-from cr.config import (
-    config,
-    config_path_list,
-    config_pureposixpath_list,
-    load_config,
-)
-from cr.rich_utils import (
-    CONSOLE,
-    CONSOLE_ERR,
-    Progress,
-    RichArgparseFormatter,
-    osc_reset,
-)
+from rich.progress import BarColumn
+from rich.progress import MofNCompleteColumn
+from rich.progress import TaskProgressColumn
+from rich.progress import TextColumn
+from rich.progress import TimeElapsedColumn
+
+from cr import DOCS_LINK
+from cr import LOGGER
+from cr import UserCancelError
+from cr import VERSION
+from cr.api import check_update
+from cr.api import Env
+from cr.api import Webapp
+from cr.config import config
+from cr.config import config_path_list
+from cr.config import config_pureposixpath_list
+from cr.config import load_config
+from cr.rich_utils import CONSOLE
+from cr.rich_utils import CONSOLE_ERR
+from cr.rich_utils import osc_reset
+from cr.rich_utils import Progress
+from cr.rich_utils import RichArgparseFormatter
 from cr.ssh import Server
-from cr.utils import git_ignored, paths_to_deploy
+from cr.utils import check_handle
+from cr.utils import git_ignored
+from cr.utils import paths_to_deploy
 
 
 class CustomArgumentParser(argparse.ArgumentParser):
     """
     Customizes the appearance of argparse help and output.
     """
 
@@ -180,14 +183,22 @@
         pass
 
     @classmethod
     def get_webapp(self, args: argparse.Namespace) -> Webapp:
         """
         Loads the Webapp and parses common arguments.
         """
+        # First check if the webapp handle could be valid.
+        # If it's not, immediately throw an error.
+        if not check_handle(args.webapp):
+            raise Exception(
+                f"Provided webapp `{args.webapp}` does not appear to be valid."
+                f" Run `cr {self.command} --help` for syntax."
+            )
+
         # Resolve path, if provided.
         extra_configs = []
         if hasattr(args, "path"):
             args.path = args.path.expanduser().resolve()
             if args.path.is_dir():
                 extra_configs = [args.path / ".cr.ini"]
 
@@ -207,15 +218,14 @@
 
     @classmethod
     def run(self, args: argparse.Namespace) -> None:
         pass
 
 
 class Deploy(Command):
-
     command = "deploy"
 
     help = "Upload the project to CodeRed Cloud and initiate a deployment."
 
     @classmethod
     def add_args(self, p: argparse.ArgumentParser):
         p.add_argument(*arg_webapp.args, **arg_webapp.kwargs)
@@ -241,15 +251,14 @@
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             MofNCompleteColumn(),
             TaskProgressColumn(),
             TimeElapsedColumn(),
             console=CONSOLE,
         ) as pbar:
-
             if not args.no_upload:
                 # Get list of paths to copy.
                 exclude = git_ignored(args.path)
                 exclude += config_path_list("deploy_exclude", args.webapp, [])
                 include = config_path_list("deploy_include", args.webapp, [])
                 files = paths_to_deploy(args.path, e=exclude, i=include)
                 s = Server(getattr(w, f"sftp_{args.env}_domain"), w.handle, "")
@@ -310,15 +319,14 @@
             )
             pbar.update(t, total=1, completed=1)
 
         CONSOLE.print(f"\nYour site is live at: {w.url}\n")
 
 
 class Restart(Command):
-
     command = "restart"
 
     help = (
         "Restart the currently running website on CodeRed Cloud. "
         "No new software is installed or updated."
     )
 
@@ -334,15 +342,14 @@
         w.api_queue_restart()
         CONSOLE.print(
             f"Restarting: {w.url}\n" "You will receive an email when complete."
         )
 
 
 class Check(Command):
-
     command = "check"
 
     help = "Check the local project for configuration errors."
 
     @classmethod
     def add_args(self, p: argparse.ArgumentParser):
         p.add_argument(*arg_webapp.args, **arg_webapp.kwargs)
@@ -353,15 +360,14 @@
     @classmethod
     def run(self, args: argparse.Namespace):
         w = self.get_webapp(args)
         w.local_check_path(args.path, CONSOLE)
 
 
 class Logs(Command):
-
     command = "logs"
 
     help = "Show the latest deployment logs."
 
     @classmethod
     def add_args(self, p: argparse.ArgumentParser):
         p.add_argument(*arg_webapp.args, **arg_webapp.kwargs)
@@ -385,15 +391,14 @@
             pbar.print(
                 "[connection closed]", markup=False, style="logging.level.info"
             )
             pbar.update(t, completed=1, total=1)
 
 
 class Download(Command):
-
     command = "download"
 
     help = (
         "Download a file or folder from CodeRed Cloud. "
         "By default this will also download all media files, "
         "which may take a long time."
     )
@@ -454,15 +459,14 @@
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             MofNCompleteColumn(),
             TaskProgressColumn(),
             TimeElapsedColumn(),
             console=CONSOLE,
         ) as pbar:
-
             s = Server(getattr(w, f"sftp_{args.env}_domain"), w.handle, "")
 
             # Get credentials and connect.
             t = pbar.add_task("Connecting", total=None)
 
             # Generate a new SFTP password from CodeRed Cloud API.
             passwd = w.api_get_sftp_password()
@@ -479,15 +483,14 @@
                 # Copy files.
                 s.get(args.remote, args.path, e=exclude, progress=pbar)
             finally:
                 s.close()
 
 
 class Upload(Command):
-
     command = "upload"
 
     help = "Upload a file or folder to CodeRed Cloud."
 
     @classmethod
     def add_args(self, p: argparse.ArgumentParser):
         p.add_argument(*arg_webapp.args, **arg_webapp.kwargs)
@@ -531,15 +534,14 @@
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             MofNCompleteColumn(),
             TaskProgressColumn(),
             TimeElapsedColumn(),
             console=CONSOLE,
         ) as pbar:
-
             # Get list of paths to copy.
             if args.path.is_dir():
                 exclude = git_ignored(args.path)
                 exclude += config_path_list("deploy_exclude", args.webapp, [])
                 include = config_path_list("deploy_include", args.webapp, [])
                 files = paths_to_deploy(args.path, e=exclude, i=include)
             else:
```

### Comparing `cr-1.5/cr/config.py` & `cr-1.6/cr/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Loads runtime variables from various config files.
 
 Copyright (c) 2022 CodeRed LLC.
 """
-from pathlib import Path, PurePosixPath
-from typing import List, Optional
 import configparser
 import os
+from pathlib import Path
+from pathlib import PurePosixPath
+from typing import List
+from typing import Optional
 
 from cr import LOGGER
 
 
 # List of config values to consider secret.
 # They should never be printed or logged.
 _SECRETS = ["token"]
@@ -30,15 +32,15 @@
             *lp,
         ]
     )
     LOGGER.info("Read config files: %s", read)
     return read
 
 
-def config(k, w: str = "cr", f: str = None) -> Optional[str]:
+def config(k, w: str = "cr", f: Optional[str] = None) -> Optional[str]:
     """
     Queries the various config files for a key ``k`` in either the default
     section [cr], or overridden in a webapp section ``w`` [``w``].
 
     Priority is as follows, each bullet in the list overriding those before it.
 
     * [cr] section in ~/.cr.ini
@@ -62,15 +64,15 @@
         val = os.environ.get(f"CR_{k.upper()}", val)
 
     LOGGER.debug("Config `%s`: `%s`", k, val)
 
     return val
 
 
-def config_bool(k, w: str = "cr", f: bool = None) -> Optional[bool]:
+def config_bool(k, w: str = "cr", f: Optional[bool] = None) -> Optional[bool]:
     """
     Queries a config and parses it as a boolean. Acceptable case-insensitive
     values are: on, off, yes, no, true, false, 0, 1
     """
     val = config(k, w)
     if val is None:
         return f
```

### Comparing `cr-1.5/cr/rich_utils.py` & `cr-1.6/cr/rich_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """
 Utilities to format program output with `rich`.
 
 Copyright (c) 2022 CodeRed LLC.
 """
-from typing import Generator, Iterable, List, Optional
 import argparse
-
-from rich.console import Console, Group, RenderableType, WINDOWS
+from typing import Generator
+from typing import Iterable
+from typing import List
+from typing import Optional
+
+from rich.console import Console
+from rich.console import Group
+from rich.console import RenderableType
+from rich.console import WINDOWS
 from rich.highlighter import RegexHighlighter
 from rich.measure import measure_renderables
 from rich.padding import Padding
 from rich.progress import Progress as _Progress
 from rich.progress import TaskID
 from rich.table import Table
 from rich.text import Text
@@ -173,23 +179,25 @@
         self,
         prog: str,
         indent_increment: int = 2,
         max_help_position: int = 38,
         width: Optional[int] = None,
     ) -> None:
         super().__init__(prog, indent_increment, max_help_position, width)
-        self._root_section.renderables = []
+        # Add a `renderables` array to store our custom rendering for the
+        # relevant sections.
+        self._root_section.renderables = []  # type: ignore[attr-defined]
 
     @property
     def renderables(self) -> List[RenderableType]:
-        return self._current_section.renderables  # type: ignore[no-any-return]
+        return self._current_section.renderables  # type: ignore[attr-defined]
 
     @property
     def _table(self) -> Table:
-        return self._current_section.table  # type: ignore[no-any-return]
+        return self._current_section.table  # type: ignore[attr-defined]
 
     def _pad(self, renderable: RenderableType) -> Padding:
         return Padding(renderable, pad=(0, 0, 0, self._current_indent))
 
     def _format_action_invocation(self, action: argparse.Action) -> str:
         if not action.option_strings or action.nargs == 0:
             action_invocation = super()._format_action_invocation(action)
@@ -221,15 +229,14 @@
             )
 
     def add_argument(self, action):
         """
         Override to not double indent subactions.
         """
         if action.help is not argparse.SUPPRESS:
-
             # find all invocations
             get_invocation = self._format_action_invocation
             # Ignore the initial invocation of subparser and get subactions
             # instead.
             if isinstance(action, argparse._SubParsersAction):
                 invocations = []
                 for subaction in action._get_subactions():
@@ -247,15 +254,15 @@
             # add the item to the list
             self._add_item(self._format_action, [action])
 
     def add_usage(
         self,
         usage: Optional[str],
         actions: Iterable[argparse.Action],
-        groups: Iterable[argparse._ArgumentGroup],
+        groups: Iterable[argparse._MutuallyExclusiveGroup],
         prefix: Optional[str] = None,
     ) -> None:
         # Do not pass prefix along... instead format it as a group title.
         super().add_usage(usage, actions, groups, prefix)
 
         if usage is not argparse.SUPPRESS:
             usage_text = self._format_usage(usage, actions, groups, prefix)
@@ -312,16 +319,16 @@
         return usage
 
     def start_section(self, heading: Optional[str]) -> None:
         super().start_section(
             heading
         )  # sets self._current_section to child section
 
-        self._current_section.renderables = []
-        self._current_section.table = Table(
+        self._current_section.renderables = []  # type: ignore[attr-defined]
+        self._current_section.table = Table(  # type: ignore[attr-defined]
             box=None,
             pad_edge=False,
             show_header=False,
             show_edge=False,
             highlight=True,
         )
         self._table.add_column(
@@ -353,16 +360,19 @@
     def format_help(self) -> str:
         out = super().format_help()
 
         # Handle ArgumentParser.add_subparsers() call to get the program name
         all_items = self._root_section.items
         if len(all_items) == 1:
             func, args = all_items[0]
-            if func == self._format_usage and not args[-1]:
-                return out  # return the program name instead of printing it
+            # If we are currently executing "format_usage()", return the program
+            # name instead of printing it. Otherwise it will print `: cr`
+            # randomly at the top of the usage section.
+            if func == self._format_usage and not list(args)[-1]:
+                return out
 
         renderables = Group(*self.renderables)
 
         def iter_tables(group: Group) -> Generator[Table, None, None]:
             for renderable in group.renderables:
                 if isinstance(renderable, Table):
                     yield renderable
```

### Comparing `cr-1.5/cr/ssh.py` & `cr-1.6/cr/ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Utilities for interacting with CodeRed Cloud host servers.
 
 Copyright (c) 2022 CodeRed LLC.
 """
-from dataclasses import dataclass
-from pathlib import Path, PurePosixPath
-from typing import List, Optional
-import stat
 import os
+import stat
+from dataclasses import dataclass
+from pathlib import Path
+from pathlib import PurePosixPath
+from typing import List
+from typing import Optional
 
-from paramiko.client import AutoAddPolicy, SSHClient
+from paramiko.client import AutoAddPolicy
+from paramiko.client import SSHClient
 from paramiko.sftp_client import SFTPClient
 from rich.progress import Progress
 
 from cr import LOGGER
 from cr.utils import EXCLUDE_DIRNAMES
 
 
@@ -76,15 +79,15 @@
             self._client = None
 
     def put(
         self,
         lp: List[Path],
         r: Path,
         s: PurePosixPath,
-        progress: Progress = None,
+        progress: Optional[Progress] = None,
     ) -> None:
         """
         Upload a list of paths ``lp``, relative to local root Path ``r`` to
         the server path ``s``. File and directory structure within ``r`` is
         mirrored to ``s``. Progress bar ``p`` is updated with a task for each
         file upload.
         """
@@ -125,15 +128,15 @@
                 progress.update(t, advance=1)
 
     def get(
         self,
         s: PurePosixPath,
         r: Path,
         e: List[PurePosixPath] = [],
-        progress: Progress = None,
+        progress: Optional[Progress] = None,
     ) -> None:
         """
         Recursively download a Path ``s`` from the server to local directory ``r``.
         File and directory structure within ``s`` is mirrored to ``r``.
         If ``s`` is a file, download it directly into ``r``.
         Do not download any directories in ``e`` (relative to ``s``).
         Progress bar ``p`` is updated with a task for each file download.
```

### Comparing `cr-1.5/cr/utils.py` & `cr-1.6/cr/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 """
 Subprocess and filesystem utilities for working with the local project.
 
 Copyright (c) 2022 CodeRed LLC.
 """
-from pathlib import Path
-from subprocess import PIPE, Popen
-from typing import IO, List, Tuple, Union
 import io
 import os
 import re
-
-from cr import LOGGER, ConfigurationError, DatabaseType
+from pathlib import Path
+from subprocess import PIPE
+from subprocess import Popen
+from typing import IO
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Union
+
+from cr import ConfigurationError
+from cr import DatabaseType
+from cr import LOGGER
 
 
 EXCLUDE_DIRNAMES = ["__pycache__", "node_modules", "htmlcov", "venv"]
 """
 List of directory names to always exclude from deployments.
 """
 
 TEMPLATE_PATH = Path(__file__).parent / "templates"
 """
 Templates directory included with this project.
 """
 
+URLSAFE_REGEX = re.compile(
+    r"^[a-zA-Z0-9]+[a-zA-Z0-9\-]+[a-zA-Z0-9]+$", flags=re.IGNORECASE
+)
+"""
+Regular expression to determine if a word is usable in DNS/URLs. Letter or
+number + at least one other letter or number or dash + letter or number.
+"""
+
 
 def get_command(program: str) -> Path:
     r"""
     Finds full path to a command on PATH given a command name.
     E.g. ``bash`` returns ``/bin/bash``;
     ``git`` might return ``C:\Program Files\Git\bin\git.exe``
 
@@ -60,16 +75,16 @@
                 return testpath
 
     raise FileNotFoundError(f"Could not find `{program}` on PATH")
 
 
 def exec_proc(
     args: List[str],
-    infile: Path = None,
-    outfile: Path = None,
+    infile: Optional[Path] = None,
+    outfile: Optional[Path] = None,
     outfile_mode: str = "w",
     ok_exit_codes: List[int] = [0],
 ) -> Tuple[int, str, str]:
     """
     Executes a process on the local machine.
 
     :param List[str] args:
@@ -149,15 +164,15 @@
     """
     _, out, err = exec_proc(["git", "branch", "--show-current"])
     branch = out.strip("\r\n")
     LOGGER.debug("Git branch `%s`.", branch)
     return branch
 
 
-def git_ignored(p: Path = None) -> List[Path]:
+def git_ignored(p: Optional[Path] = None) -> List[Path]:
     """
     Returns a list of absolute file and directory paths ignored by git.
     """
     lp: List[Path] = []
 
     # Build the command.
     cmd = ["git", "ls-files", "--others", "--directory"]
@@ -208,15 +223,14 @@
     will still be ignored.
 
     Any file paths in the returned list must also include their parent directory
     paths within ``r``, so that consumers of this list will know to create them.
     """
     lp: List[Path] = []
     for root, dirs, files in os.walk(r):
-
         # If subdir is excluded, delete it from the list, so ``os`` will not
         # traverse it. Otherwise, append to the list.
         dirs_copy = dirs.copy()
         for d in dirs_copy:
             dp = Path(os.path.join(root, d))
             dpr = dp.resolve()
             # Force add if included.
@@ -257,14 +271,28 @@
 def template(t: str) -> str:
     """
     Read file ``t`` from the templates directory and return it as a string.
     """
     return (TEMPLATE_PATH / t).read_text()
 
 
+def is_urlsafe(value: str) -> bool:
+    """
+    Determines if value is a valid URL, subdomain, etc.
+    """
+    return bool(URLSAFE_REGEX.match(value))
+
+
+def check_handle(value: str) -> bool:
+    """
+    Check if the provided ``value`` could be a valid webapp handle.
+    """
+    return is_urlsafe(value) and len(value) <= 32
+
+
 def django_manage_check(p: Path) -> None:
     if not (p / "manage.py").is_file():
         raise FileNotFoundError("manage.py")
 
 
 def django_requirements_check(p: Path) -> None:
     if not (p / "requirements.txt").is_file():
```

### Comparing `cr-1.5/cr.egg-info/PKG-INFO` & `cr-1.6/cr.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: cr
-Version: 1.5
-Summary: The official CodeRed Cloud command line tool.
-Author-email: CodeRed LLC <info@coderedcorp.com>
-License: MIT License
-        
-        Copyright (c) 2022 CodeRed LLC
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://www.codered.cloud/cli/
-Project-URL: Source, https://github.com/coderedcorp/cr
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-`cr` - CodeRed Cloud CLI
-========================
-
-The official CodeRed Cloud command line tool. Easily deploy your Django, Wagtail, WordPress, or Static HTML sites directly from your terminal or version control system.
-
-https://www.codered.cloud/cli/
-
----
-
-To contribute, see the [CONTRIBUTING.md](CONTRIBUTING.md) file in this repository.
+Metadata-Version: 2.1
+Name: cr
+Version: 1.6
+Summary: The official CodeRed Cloud command line tool.
+Author-email: CodeRed LLC <info@coderedcorp.com>
+License: MIT License
+        
+        Copyright (c) 2022 CodeRed LLC
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://www.codered.cloud/cli/
+Project-URL: Source, https://github.com/coderedcorp/cr
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+`cr` - CodeRed Cloud CLI
+========================
+
+The official CodeRed Cloud command line tool. Easily deploy your Django, Wagtail, WordPress, or Static HTML sites directly from your terminal or version control system.
+
+https://www.codered.cloud/cli/
+
+---
+
+To contribute, see the [CONTRIBUTING.md](CONTRIBUTING.md) file in this repository.
```

### Comparing `cr-1.5/pyproject.toml` & `cr-1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ]
 classifiers = [
     "Environment :: Console",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "certifi",
-    "paramiko==2.11.*",
-    "rich==12.6.*",
+    "paramiko==3.2.*",
+    "rich==13.4.*",
 ]
 description = "The official CodeRed Cloud command line tool."
 dynamic = ["version"]
 license = {file = "LICENSE.txt"}
 name = "cr"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.scripts]
 cr = "cr.cli:main"
 
 [project.urls]
 Homepage = "https://www.codered.cloud/cli/"
 Source = "https://github.com/coderedcorp/cr"
@@ -46,20 +46,29 @@
 [tool.coverage.run]
 source = ["cr"]
 omit = [
     ".*",
     "venv/*",
 ]
 
-[tool.pytest.ini_options]
-addopts = "--cov cr --cov-report html"
+[tool.isort]
+force_alphabetical_sort_within_sections = true
+force_single_line = true
+lines_after_imports = 2
+lines_between_sections = 1
+line_length = 80
+profile = "black"
+skip_gitignore = true
 
 [tool.mypy]
 ignore_missing_imports = true
 
+[tool.pytest.ini_options]
+addopts = "--cov cr --cov-report html"
+
 [tool.setuptools]
 packages = ["cr", "cr.templates"]
 
 [tool.setuptools.package-data]
 "cr.templates" = ["*"]
 
 [tool.setuptools.dynamic]
```

