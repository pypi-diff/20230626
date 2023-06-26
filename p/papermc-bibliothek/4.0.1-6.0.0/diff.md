# Comparing `tmp/papermc-bibliothek-4.0.1.tar.gz` & `tmp/papermc_bibliothek-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermc-bibliothek-4.0.1.tar", max compression
+gzip compressed data, was "papermc_bibliothek-6.0.0.tar", max compression
```

## Comparing `papermc-bibliothek-4.0.1.tar` & `papermc_bibliothek-6.0.0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0     1064 2022-04-11 10:22:56.963496 papermc-bibliothek-4.0.1/LICENSE
--rw-r--r--   0        0        0     1190 2022-04-12 16:12:29.681185 papermc-bibliothek-4.0.1/README.md
--rw-r--r--   0        0        0       25 2022-08-23 18:50:49.919559 papermc-bibliothek-4.0.1/bibliothek/__init__.py
--rw-r--r--   0        0        0     4393 2022-08-23 19:13:55.201162 papermc-bibliothek-4.0.1/bibliothek/__main__.py
--rw-r--r--   0        0        0    10692 2022-08-23 19:17:43.129477 papermc-bibliothek-4.0.1/bibliothek/bibliothek.py
--rw-r--r--   0        0        0      714 2022-08-23 19:27:35.399901 papermc-bibliothek-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     2122 2022-08-23 19:28:01.295027 papermc-bibliothek-4.0.1/setup.py
--rw-r--r--   0        0        0     1925 2022-08-23 19:28:01.295212 papermc-bibliothek-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-04-11 10:22:56.963000 papermc_bibliothek-6.0.0/LICENSE
+-rw-r--r--   0        0        0      922 2023-06-26 01:17:34.738999 papermc_bibliothek-6.0.0/README.md
+-rw-r--r--   0        0        0       26 2023-06-26 01:48:16.672464 papermc_bibliothek-6.0.0/bibliothek/__init__.py
+-rw-r--r--   0        0        0    11472 2023-06-26 01:44:30.731748 papermc_bibliothek-6.0.0/bibliothek/bibliothek.py
+-rw-r--r--   0        0        0      601 2023-06-26 01:15:07.289117 papermc_bibliothek-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 papermc_bibliothek-6.0.0/PKG-INFO
```

### Comparing `papermc-bibliothek-4.0.1/LICENSE` & `papermc_bibliothek-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `papermc-bibliothek-4.0.1/README.md` & `papermc_bibliothek-6.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,36 @@
 # papermc-bibliothek
 
-pythonic [bibliothek](https://github.com/PaperMC/bibliothek) API wrapper with a CLI
+pythonic [bibliothek](https://github.com/PaperMC/bibliothek) API wrapper
 
 ## Installation
 
 papermc-bibliothek requires python 3.9 or above
 
 ```shell
-# PIP3
-pip3 install papermc-bibliothek
-# PIP
 pip install papermc-bibliothek
 ```
 
+```shell
+poetry add papermc-bibliothek
+```
+
 ## API
 
 All functions and classes are properly type hinted and documented with triple quotes. Please file an issue or pull
 request with any corrections if any issues are found.
 
+You can refer to https://papermc.io/api if looking for a specific
+method, they are named similarly.
+
 ### Basic Usage
 
 ```python
 from bibliothek import Bibliothek, BibliothekException
 
 bibliothek = Bibliothek()  # Create an instance of the Bibliothek class
 try:
     projects = bibliothek.get_projects()
     print(projects)  # ['paper', 'travertine', 'waterfall', 'velocity']
 except BibliothekException as e:  # Catch BibliothekException in case something goes wrong
     print(f"Error: {e}")
-```
-
-## CLI
-
-Will generally contain most features of the API<!--, use (the secret project) for proper server managment-->.
-
-```shell
-Usage: bibliothek [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  download-build
-  get-build
-  get-project
-  get-projects
-  get-version
-  get-version-group
-  get-version-group-builds
 ```
```

### Comparing `papermc-bibliothek-4.0.1/bibliothek/bibliothek.py` & `papermc_bibliothek-6.0.0/bibliothek/bibliothek.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 import datetime
 import hashlib
 import importlib.metadata
 import json
 from io import BytesIO
 from json import JSONDecodeError
-from typing import List, Dict
+from typing import List, Dict, Callable
 
 import dateutil.parser
 import urllib3
 
 try:
     __version__ = importlib.metadata.version('papermc-bibliothek')
 except importlib.metadata.PackageNotFoundError:
@@ -92,26 +92,26 @@
 
 
 class BibliothekException(Exception):
     pass
 
 
 class UnexpectedResponseBibliothekException(Exception):
-    def __init__(self, response: urllib3.response.HTTPResponse):
-        self.response: urllib3.response.HTTPResponse = response
+    def __init__(self, response: urllib3.response.BaseHTTPResponse):
+        self.response = response
 
         self._end = self.response.data
 
         if self.response.status == 404:
             try:
                 self._end = "Error: " + json.loads(self._end.decode('utf-8'))["error"]
             except JSONDecodeError:
                 self._end = "Data: " + str(self._end)
         else:
-            self._end = "Data: " + self._end
+            self._end = "Data: " + str(self._end)
 
         super().__init__()
 
     def __str__(self):
         return f"HTTP Code: {self.response.status}, expected 200. {self._end}"
 
 
@@ -140,69 +140,76 @@
         return downloads
 
     def get_projects(self) -> List[str]:
         """
         Get the list of projects
         :return: A List of projects
         """
-        response = self.pool_manager.request("GET", f"{self.base_url}projects")
+        url = f"{self.base_url}projects"
+        response = self.pool_manager.request("GET", url)
         if response.status != 200:
             raise UnexpectedResponseBibliothekException(response)
 
-        return json.loads(response.data)["projects"]
+        return response.json()["projects"]
 
     def get_project(self, project_id: str) -> BibliothekProject:
         """
         Get a bibliothek project
         :param project_id: a valid bibliothek project id
         :return: The bibliothek project
         """
-        response = self.pool_manager.request("GET", f"{self.base_url}projects/{project_id}")
+
+        # https://papermc.io/api/docs/swagger-ui/index.html?configUrl=/api/openapi/swagger-config#/projects-controller/projects
+        url = f"{self.base_url}projects/{project_id}"
+        response = self.pool_manager.request("GET", url)
         if response.status != 200:
-            raise UnexpectedResponseBibliothekException(response.status)
+            raise UnexpectedResponseBibliothekException(response)
 
-        project_dict = json.loads(response.data)
+        project_dict = response.json()
 
         return BibliothekProject(project_dict["project_id"], project_dict["project_name"],
                                  project_dict["version_groups"], project_dict["versions"])
 
     def get_version_group(self, project_id: str, version_group: str) -> BibliothekVersionGroup:
         """
         Get a version group
         :param project_id: a valid bibliothek project id
         :param version_group: a valid bibliothek version group
         :return: A bibliothek version group object
         """
-        response = self.pool_manager.request("GET",
-                                             f"{self.base_url}projects/{project_id}/version_group/{version_group}")
+
+        # https://papermc.io/api/docs/swagger-ui/index.html?configUrl=/api/openapi/swagger-config#/project-controller/project
+        url = f"{self.base_url}projects/{project_id}/version_group/{version_group}"
+        response = self.pool_manager.request("GET", url)
         if response.status != 200:
             raise UnexpectedResponseBibliothekException(response)
 
-        version_group_dict = json.loads(response.data)
+        version_group_dict = response.json()
 
         return BibliothekVersionGroup(version_group_dict["project_id"], version_group_dict["project_name"],
                                       version_group_dict["version_group"], version_group_dict["versions"])
 
     def get_version_group_builds(self, project_id: str, version_group: str) -> BibliothekVersionGroupBuilds:
         """
         Get the builds for a bibliothek version group
         :param project_id: a valid bibliothek project id
         :param version_group: a valid version group
         :return: a bibliothek version group builds object
         """
-        response: urllib3.response.HTTPResponse = self.pool_manager.request("GET",
-                                                                            f"{self.base_url}projects/{project_id}/version_group/{version_group}/builds")
+
+        # https://papermc.io/api/docs/swagger-ui/index.html?configUrl=/api/openapi/swagger-config#/version-family-builds-controller/familyBuilds
+        url = f"{self.base_url}projects/{project_id}/version_group/{version_group}/builds"
+        response = self.pool_manager.request("GET", url)
         if response.status != 200:
             raise UnexpectedResponseBibliothekException(response)
 
-        version_group_builds_dict = json.loads(response.data)
+        version_group_builds_dict = response.json()
 
         builds = []
-        for build in version_group_builds_dict[
-            "builds"]:
+        for build in version_group_builds_dict["builds"]:
             builds.append(
                 BibliothekVersionGroupBuild(build["version"], build["build"], dateutil.parser.parse(build["time"]),
                                             build["channel"], build["promoted"],
                                             self._change_data_list_to_change_list(build["changes"]),
                                             self._download_data_dict_to_download_dict(build["downloads"])))
 
         return BibliothekVersionGroupBuilds(version_group_builds_dict["project_id"],
@@ -213,64 +220,73 @@
     def get_version_builds(self, project_id: str, version: str) -> BibliothekVersionBuilds:
         """
         Get a bibliothek version
         :param project_id: a valid bibliothek project id
         :param version: a valid version for the provided project id
         :return: a bibliothek version object
         """
-        response = self.pool_manager.request("GET",
-                                             f"{self.base_url}projects/{project_id}/versions/{version}")
+
+        # https://papermc.io/api/docs/swagger-ui/index.html?configUrl=/api/openapi/swagger-config#/version-builds-controller/builds
+        url = f"{self.base_url}projects/{project_id}/versions/{version}"
+        response = self.pool_manager.request("GET", url)
         if response.status != 200:
             raise UnexpectedResponseBibliothekException(response)
 
-        version_dict = json.loads(response.data)
+        version_dict = response.json()
 
         return BibliothekVersionBuilds(version_dict["project_id"], version_dict["project_name"],
                                        version_dict["version"], version_dict["builds"])
 
     def get_build(self, project_id: str, version: str, build: int) -> BibliothekBuild:
         """
         get a specific build
         :param project_id: a valid bibliothek project id
         :param version: a valid bibliothek version for the project id
         :param build: a valid bibliothek build for the version on the project
         :return: a bibliothek build object
         """
-        response: urllib3.response.HTTPResponse = self.pool_manager.request("GET",
-                                                                            f"{self.base_url}projects/{project_id}/versions/{version}/builds/{build}")
+
+        # https://papermc.io/api/docs/swagger-ui/index.html?configUrl=/api/openapi/swagger-config#/version-build-controller/build
+        url = f"{self.base_url}projects/{project_id}/versions/{version}/builds/{build}"
+        response = self.pool_manager.request("GET", url)
         if response.status != 200:
             raise UnexpectedResponseBibliothekException(response)
 
-        build_dict = json.loads(response.data)
+        build_dict = response.json()
 
         return BibliothekBuild(build_dict["project_id"], build_dict["project_name"],
                                build_dict["version"], build_dict["build"], dateutil.parser.parse(build_dict["time"]),
                                build_dict["channel"], build_dict["promoted"],
                                self._change_data_list_to_change_list(build_dict["changes"]),
                                self._download_data_dict_to_download_dict(build_dict["downloads"]))
 
-    def download_build(self, project_id: str, version: str, build: int, filename: str) -> BytesIO:
+    def download_build(self, project_id: str, version: str, build: int, filename: str,
+                       progress_callback: Callable[[int, int or None], None] = None) -> BytesIO:
         """
         downloads a build
         :param project_id: a valid bibliothek project id
         :param version: a valid bibliothek version for the project
         :param build: a valid bibliothek build
         :param filename: the name of the download, eg: `paper-1.18.2-286.jar`
+        :param progress_callback: A callback for when the download advances. Params (in bytes): downloaded, total
         :return: A BytesIO object with the download
         """
-        request = self.pool_manager.request("GET",
-                                            f"{self.base_url}projects/{project_id}/versions/{version}/builds/{build}/downloads/{filename}",
-                                            preload_content=False)
+
+        # https://papermc.io/api/docs/swagger-ui/index.html?configUrl=/api/openapi/swagger-config#/download-controller/download
+        url = f"{self.base_url}projects/{project_id}/versions/{version}/builds/{build}/downloads/{filename}"
+        request = self.pool_manager.request("GET", url, preload_content=False)
 
         download_bytesio = BytesIO()
         while True:
             data = request.read(2 ** 16)  # 64kb
             if not data:
                 break
             download_bytesio.write(data)
+            if progress_callback:
+                progress_callback(download_bytesio.getbuffer().nbytes, request.headers.get("Content-Length"))
 
         request.release_conn()
 
         if request.status != 200:
             raise UnexpectedResponseBibliothekException(request)
 
         return download_bytesio
```

### Comparing `papermc-bibliothek-4.0.1/pyproject.toml` & `papermc_bibliothek-6.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 [tool.poetry]
 name = "papermc-bibliothek"
 packages = [{ include = "bibliothek" }]
-version = "4.0.1"
+version = "6.0.0"
 description = "bibliothek API client with CLI"
 authors = ["Oskar <56176746+OskarZyg@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/OskarsMC-Network/papermc-bibliothek"
 homepage = "https://github.com/OskarsMC-Network/papermc-bibliothek"
 
-[tool.poetry.scripts]
-bibliothek = "bibliothek.__main__:app"
-
 [tool.poetry.dependencies]
 python = "^3.9"
-typer = { extras = ["all"], version = "^0.6.1" }
-urllib3 = "^1.26.12"
 python-dateutil = "^2.8.2"
+urllib3 = "^2.0.3"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `papermc-bibliothek-4.0.1/PKG-INFO` & `papermc_bibliothek-6.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,55 @@
 Metadata-Version: 2.1
 Name: papermc-bibliothek
-Version: 4.0.1
+Version: 6.0.0
 Summary: bibliothek API client with CLI
 Home-page: https://github.com/OskarsMC-Network/papermc-bibliothek
 License: MIT
 Author: Oskar
 Author-email: 56176746+OskarZyg@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
-Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
+Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/OskarsMC-Network/papermc-bibliothek
 Description-Content-Type: text/markdown
 
 # papermc-bibliothek
 
-pythonic [bibliothek](https://github.com/PaperMC/bibliothek) API wrapper with a CLI
+pythonic [bibliothek](https://github.com/PaperMC/bibliothek) API wrapper
 
 ## Installation
 
 papermc-bibliothek requires python 3.9 or above
 
 ```shell
-# PIP3
-pip3 install papermc-bibliothek
-# PIP
 pip install papermc-bibliothek
 ```
 
+```shell
+poetry add papermc-bibliothek
+```
+
 ## API
 
 All functions and classes are properly type hinted and documented with triple quotes. Please file an issue or pull
 request with any corrections if any issues are found.
 
+You can refer to https://papermc.io/api if looking for a specific
+method, they are named similarly.
+
 ### Basic Usage
 
 ```python
 from bibliothek import Bibliothek, BibliothekException
 
 bibliothek = Bibliothek()  # Create an instance of the Bibliothek class
 try:
     projects = bibliothek.get_projects()
     print(projects)  # ['paper', 'travertine', 'waterfall', 'velocity']
 except BibliothekException as e:  # Catch BibliothekException in case something goes wrong
     print(f"Error: {e}")
 ```
-
-## CLI
-
-Will generally contain most features of the API<!--, use (the secret project) for proper server managment-->.
-
-```shell
-Usage: bibliothek [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  download-build
-  get-build
-  get-project
-  get-projects
-  get-version
-  get-version-group
-  get-version-group-builds
-```
```

