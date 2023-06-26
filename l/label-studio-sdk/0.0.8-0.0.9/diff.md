# Comparing `tmp/label-studio-sdk-0.0.8.tar.gz` & `tmp/label-studio-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/label-studio-sdk-0.0.8.tar", last modified: Wed Jan 19 21:00:54 2022, max compression
+gzip compressed data, was "dist/label-studio-sdk-0.0.9.tar", last modified: Tue Feb  8 20:57:32 2022, max compression
```

## Comparing `label-studio-sdk-0.0.8.tar` & `label-studio-sdk-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/
--rw-r--r--   0 nik        (503) staff       (20)       25 2021-11-12 14:56:27.000000 label-studio-sdk-0.0.8/MANIFEST.in
--rw-r--r--   0 nik        (503) staff       (20)      497 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 nik        (503) staff       (20)     3722 2021-11-12 14:56:27.000000 label-studio-sdk-0.0.8/README.md
-drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/docs/
--rw-r--r--   0 nik        (503) staff       (20)       32 2021-11-08 20:12:01.000000 label-studio-sdk-0.0.8/docs/__init__.py
-drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/label_studio_sdk/
--rw-r--r--   0 nik        (503) staff       (20)      149 2022-01-19 21:00:50.000000 label-studio-sdk-0.0.8/label_studio_sdk/__init__.py
--rw-r--r--   0 nik        (503) staff       (20)     6429 2022-01-18 22:06:47.000000 label-studio-sdk-0.0.8/label_studio_sdk/client.py
--rw-r--r--   0 nik        (503) staff       (20)     8035 2021-12-18 14:22:31.000000 label-studio-sdk-0.0.8/label_studio_sdk/data_manager.py
--rw-r--r--   0 nik        (503) staff       (20)    48128 2021-12-18 14:22:31.000000 label-studio-sdk-0.0.8/label_studio_sdk/project.py
--rw-r--r--   0 nik        (503) staff       (20)     1325 2022-01-14 11:21:11.000000 label-studio-sdk-0.0.8/label_studio_sdk/users.py
--rw-r--r--   0 nik        (503) staff       (20)     4083 2021-11-08 20:12:01.000000 label-studio-sdk-0.0.8/label_studio_sdk/utils.py
--rw-r--r--   0 nik        (503) staff       (20)     1163 2022-01-18 22:06:37.000000 label-studio-sdk-0.0.8/label_studio_sdk/workspaces.py
-drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/label_studio_sdk.egg-info/
--rw-r--r--   0 nik        (503) staff       (20)      497 2022-01-19 21:00:53.000000 label-studio-sdk-0.0.8/label_studio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 nik        (503) staff       (20)      502 2022-01-19 21:00:53.000000 label-studio-sdk-0.0.8/label_studio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (503) staff       (20)        1 2022-01-19 21:00:53.000000 label-studio-sdk-0.0.8/label_studio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (503) staff       (20)       81 2022-01-19 21:00:53.000000 label-studio-sdk-0.0.8/label_studio_sdk.egg-info/requires.txt
--rw-r--r--   0 nik        (503) staff       (20)       28 2022-01-19 21:00:53.000000 label-studio-sdk-0.0.8/label_studio_sdk.egg-info/top_level.txt
--rw-r--r--   0 nik        (503) staff       (20)       80 2022-01-18 22:06:47.000000 label-studio-sdk-0.0.8/requirements.txt
--rw-r--r--   0 nik        (503) staff       (20)       38 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/setup.cfg
--rw-r--r--   0 nik        (503) staff       (20)     1143 2021-11-12 14:56:27.000000 label-studio-sdk-0.0.8/setup.py
-drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-01-19 21:00:54.000000 label-studio-sdk-0.0.8/tests/
--rw-r--r--   0 nik        (503) staff       (20)        0 2022-01-18 22:06:47.000000 label-studio-sdk-0.0.8/tests/__init__.py
--rw-r--r--   0 nik        (503) staff       (20)      913 2022-01-18 22:06:47.000000 label-studio-sdk-0.0.8/tests/test_client.py
+drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/
+-rw-r--r--   0 nik        (503) staff       (20)    11342 2021-11-08 20:12:01.000000 label-studio-sdk-0.0.9/LICENSE
+-rw-r--r--   0 nik        (503) staff       (20)       25 2021-11-12 14:56:27.000000 label-studio-sdk-0.0.9/MANIFEST.in
+-rw-r--r--   0 nik        (503) staff       (20)      497 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 nik        (503) staff       (20)     3722 2021-11-12 14:56:27.000000 label-studio-sdk-0.0.9/README.md
+drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/docs/
+-rw-r--r--   0 nik        (503) staff       (20)       32 2021-11-08 20:12:01.000000 label-studio-sdk-0.0.9/docs/__init__.py
+drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/label_studio_sdk/
+-rw-r--r--   0 nik        (503) staff       (20)      149 2022-02-08 20:57:13.000000 label-studio-sdk-0.0.9/label_studio_sdk/__init__.py
+-rw-r--r--   0 nik        (503) staff       (20)     8055 2022-02-08 20:56:17.000000 label-studio-sdk-0.0.9/label_studio_sdk/client.py
+-rw-r--r--   0 nik        (503) staff       (20)     8035 2021-12-18 14:22:31.000000 label-studio-sdk-0.0.9/label_studio_sdk/data_manager.py
+-rw-r--r--   0 nik        (503) staff       (20)    55447 2022-02-08 20:56:17.000000 label-studio-sdk-0.0.9/label_studio_sdk/project.py
+-rw-r--r--   0 nik        (503) staff       (20)     1325 2022-01-14 11:21:11.000000 label-studio-sdk-0.0.9/label_studio_sdk/users.py
+-rw-r--r--   0 nik        (503) staff       (20)     4083 2021-11-08 20:12:01.000000 label-studio-sdk-0.0.9/label_studio_sdk/utils.py
+-rw-r--r--   0 nik        (503) staff       (20)     1163 2022-01-18 22:06:37.000000 label-studio-sdk-0.0.9/label_studio_sdk/workspaces.py
+drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/label_studio_sdk.egg-info/
+-rw-r--r--   0 nik        (503) staff       (20)      497 2022-02-08 20:57:31.000000 label-studio-sdk-0.0.9/label_studio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (503) staff       (20)      510 2022-02-08 20:57:31.000000 label-studio-sdk-0.0.9/label_studio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (503) staff       (20)        1 2022-02-08 20:57:31.000000 label-studio-sdk-0.0.9/label_studio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (503) staff       (20)       48 2022-02-08 20:57:31.000000 label-studio-sdk-0.0.9/label_studio_sdk.egg-info/requires.txt
+-rw-r--r--   0 nik        (503) staff       (20)       28 2022-02-08 20:57:31.000000 label-studio-sdk-0.0.9/label_studio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 nik        (503) staff       (20)       48 2022-02-08 20:56:13.000000 label-studio-sdk-0.0.9/requirements.txt
+-rw-r--r--   0 nik        (503) staff       (20)       38 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 nik        (503) staff       (20)     1143 2021-11-12 14:56:27.000000 label-studio-sdk-0.0.9/setup.py
+drwxr-xr-x   0 nik        (503) staff       (20)        0 2022-02-08 20:57:32.000000 label-studio-sdk-0.0.9/tests/
+-rw-r--r--   0 nik        (503) staff       (20)        0 2022-01-18 22:06:47.000000 label-studio-sdk-0.0.9/tests/__init__.py
+-rw-r--r--   0 nik        (503) staff       (20)      913 2022-01-18 22:06:47.000000 label-studio-sdk-0.0.9/tests/test_client.py
```

### Comparing `label-studio-sdk-0.0.8/README.md` & `label-studio-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `label-studio-sdk-0.0.8/label_studio_sdk/client.py` & `label-studio-sdk-0.0.9/label_studio_sdk/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,79 @@
 """ .. include::../docs/client.md
 """
-import requests
+import warnings
 import logging
+import requests
 
+from typing import Optional
+from pydantic import BaseModel, constr, root_validator
 from requests.adapters import HTTPAdapter
 
 logger = logging.getLogger(__name__)
 
 MAX_RETRIES = 3
 TIMEOUT = (1.0, 60.0)
 HEADERS = {}
 
 
+class ClientCredentials(BaseModel):
+    email: Optional[str]
+    password: Optional[str]
+    api_key: Optional[constr()] = None
+
+    @root_validator(pre=True, allow_reuse=True)
+    def either_key_or_email_password(cls, values):
+        assert 'email' in values or 'api_key' in values, 'At least one of email or api_key should be included'
+        assert 'email' not in values or 'password' in values, 'Provide both email and password for login auth'
+        return values
+
+
 class Client(object):
 
-    def __init__(self, url, api_key, session=None, extra_headers: dict = None):
+    def __init__(self, url, api_key, credentials=None, session=None, extra_headers: dict = None):
         """ Initialize the client. Do this before using other Label Studio SDK classes and methods in your script.
 
         Parameters
         ----------
         url: str
             Label Studio host address.
             Example: http://localhost:8080
         api_key: str
             User token for the API. You can find this on your user account page in Label Studio.
+        credentials: ClientCredentials
+            User email and password or api_key.
         session: requests.Session()
             If None, a new one is created.
         extra_headers: dict
             Additional headers that will be passed to each http request
         """
         self.url = url.rstrip('/')
-        self.api_key = api_key
         self.session = session or self.get_session()
+         
+        # set api key or get it using credentials (username and password)
+        if api_key is not None:
+            warnings.warn("A deprecation warning to fit accordingly to your deprecation policy", DeprecationWarning)
+            credentials = ClientCredentials(api_key=api_key)
+        self.api_key = credentials.api_key if credentials.api_key else self.get_api_key(credentials)
+
+        # set headers
         self.headers = {'Authorization': f'Token {self.api_key}'}
         if extra_headers:
             self.headers.update(extra_headers)
 
+    def get_api_key(self, credentials: ClientCredentials):
+        login_url = self.get_url("/user/login")
+        # Retrieve and set the CSRF token first
+        self.session.get(login_url)
+        csrf_token = self.session.cookies.get('csrftoken', None)
+        login_data = dict(**credentials.dict(), csrfmiddlewaretoken=csrf_token)
+        self.session.post(login_url, data=login_data, headers=dict(Referer=self.url)).raise_for_status()
+        api_key = self.session.get(self.get_url("/api/current-user/token")).json().get("token")
+        return api_key
+
     def check_connection(self):
         """ Call Label Studio /health endpoint to check the connection to the server.
 
         Returns
         -------
         dict
             Status string like "UP"
```

### Comparing `label-studio-sdk-0.0.8/label_studio_sdk/data_manager.py` & `label-studio-sdk-0.0.9/label_studio_sdk/data_manager.py`

 * *Files identical despite different names*

### Comparing `label-studio-sdk-0.0.8/label_studio_sdk/project.py` & `label-studio-sdk-0.0.9/label_studio_sdk/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ .. include::../docs/project.md
 """
 import os
-import time
 import json
 
-from enum import Enum
-from typing import Optional, Union, List, Dict
+from enum import Enum, auto
+from random import sample, shuffle
+from typing import Optional, Union, List, Dict, Callable
 from .client import Client
 from .utils import parse_config
 
 
 class LabelStudioException(Exception):
     pass
 
@@ -44,14 +44,18 @@
     """ Label Studio Local File Storage """
     REDIS = 'redis'
     """ Redis Storage """
     S3_SECURED = 's3s'
     """ Amazon S3 Storage secured by IAM roles (Enterprise only)"""
 
 
+class AssignmentSamplingMethod(Enum):
+    RANDOM = auto()  # produces uniform splits across annotators
+
+
 class Project(Client):
 
     def __init__(self, *args, **kwargs):
         """ Initialize project class.
 
         Parameters
         ----------
@@ -85,14 +89,33 @@
                 "labels": ["Label1", "Label2", "Label3"]
         }
         ```
         `"labels"` are taken from "alias" attribute if it exists, else "value"
         """
         return parse_config(self.label_config)
 
+    def get_members(self):
+        """ Get members from this project.
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        list of `label_studio_sdk.users.User`
+
+        """
+        from .users import User
+        response = self.make_request('GET', f'/api/projects/{self.id}/members')
+        users = []
+        for user_data in response.json():
+            user_data['client'] = self
+            users.append(User(**user_data))
+        return users
+
     def add_member(self, user):
         """ Add a user to a project.
 
         Parameters
         ----------
         user: User
 
@@ -637,14 +660,48 @@
     def get_paginated_tasks_ids(self, *args, **kwargs):
         """Same as `label_studio_sdk.project.Project.get_paginated_tasks()` but returns
            only task IDs.
         """
         kwargs['only_ids'] = True
         return self.get_paginated_tasks(*args, **kwargs)
 
+    def get_views(self):
+        """Get all views related to the project
+
+        Returns
+        -------
+        list
+            List of view dicts
+        """
+        response = self.make_request('GET', f'/api/dm/views?project={self.id}')
+        return response.json()
+
+    def create_view(self, filters):
+        """Create view
+
+        Parameters
+        ----------
+        filters: dict
+            Specify the filters(`label_studio_sdk.data_manager.Filters`) of the view
+
+        Returns
+        -------
+        dict:
+            dict with created view
+
+        """
+        data = {
+            'project': self.id,
+            'data': {
+                'filters': filters,
+            }
+        }
+        response = self.make_request('POST', '/api/dm/views', json=data)
+        return response.json()
+
     @property
     def tasks(self):
         """ Retrieve all tasks from the project. This call can be very slow if the project has a lot of tasks.
         """
         return self.get_tasks()
 
     @property
@@ -1323,7 +1380,153 @@
             'title': title,
             'description': description,
             'can_delete_objects': can_delete_objects,
             'project': self.id
         }
         response = self.make_request('POST', '/api/storages/export/azure', json=payload)
         return response.json()
+
+    def _assign_by_sampling(
+            self,
+            users: List[int],
+            assign_function: Callable,
+            view_id: int = None,
+            method: AssignmentSamplingMethod = AssignmentSamplingMethod.RANDOM,
+            fraction: float = 1.0,
+            overlap: int = 1
+    ):
+        """
+        Assigning tasks to Reviewers or Annotators by assign_function with method by fraction from view_id
+        Parameters
+        ----------
+        users: List[int]
+            users' IDs list
+        assign_function: Callable
+            Function to assign tasks by list of user IDs
+        view_id: int
+            Optional, view ID to filter tasks to assign
+        method: AssignmentSamplingMethod
+            Optional, Assignment method
+        fraction: float
+            Optional, expresses the size of dataset to be assigned
+        overlap: int
+            Optional, expresses the count of assignments for each task
+        Returns
+        -------
+        list[dict]
+            List of dicts with counter of created assignments
+        """
+        assert len(users) > 0, 'Users list is empty.'
+        assert len(users) >= overlap, 'Overlap is more than number of users.'
+        final_results = []
+        # Get tasks to assign
+        tasks = self.get_tasks(view_id=view_id, only_ids=True)
+        assert len(tasks) > 0, 'Tasks list is empty.'
+        # Choice fraction of tasks
+        if fraction != 1.0:
+            k = int(len(tasks) * fraction)
+            tasks = sample(tasks, k)
+        # prepare random list of tasks for overlap > 1
+        if overlap > 1:
+            shuffle(tasks)
+            tasks = tasks * overlap
+        # Check how many tasks for each user
+        n_tasks = max(int(len(tasks) / len(users)), 1)
+        # Assign each user tasks
+        for user in users:
+            # check if last chunk of tasks is less than average chunk
+            if n_tasks > len(tasks):
+                n_tasks = len(tasks)
+            # check if last chunk of tasks is more than average chunk + 1
+            # (covers rounding issue in line 1407)
+            elif n_tasks + 1 == len(tasks) and n_tasks != 1:
+                n_tasks = n_tasks + 1
+            if method == AssignmentSamplingMethod.RANDOM and overlap == 1:
+                sample_tasks = sample(tasks, n_tasks)
+            elif method == AssignmentSamplingMethod.RANDOM and overlap > 1:
+                sample_tasks = tasks[:n_tasks]
+            else:
+                raise ValueError(f"Sampling method {method} is not allowed")
+            final_results.append(assign_function([user], sample_tasks))
+            if overlap > 1:
+                tasks = tasks[n_tasks:]
+            else:
+                tasks = list(set(tasks) - set(sample_tasks))
+            if len(tasks) == 0:
+                break
+        # check if any tasks left
+        if len(tasks) > 0:
+            final_results.append(assign_function([users[-1]], tasks))
+        return final_results
+
+    def assign_reviewers_by_sampling(
+            self,
+            users: List[int],
+            view_id: int = None,
+            method: AssignmentSamplingMethod = AssignmentSamplingMethod.RANDOM,
+            fraction: float = 1.0,
+            overlap: int = 1
+    ):
+        """
+        Behaves similarly like `assign_reviewers()` but instead of specify tasks_ids explicitely,
+        it gets users' IDs list and optional view ID and uniformly splits all tasks across reviewers
+        Fraction expresses the size of dataset to be assigned
+        Parameters
+        ----------
+        users: List[int]
+            users' IDs list
+        view_id: int
+            Optional, view ID to filter tasks to assign
+        method: AssignmentSamplingMethod
+            Optional, Assignment method
+        fraction: float
+            Optional, expresses the size of dataset to be assigned
+        overlap: int
+            Optional, expresses the count of assignments for each task
+        Returns
+        -------
+        list[dict]
+            List of dicts with counter of created assignments
+        """
+
+        return self._assign_by_sampling(users=users,
+                                        assign_function=self.assign_reviewers,
+                                        view_id=view_id,
+                                        method=method,
+                                        fraction=fraction,
+                                        overlap=overlap)
+
+    def assign_annotators_by_sampling(
+            self,
+            users: List[int],
+            view_id: int = None,
+            method: AssignmentSamplingMethod = AssignmentSamplingMethod.RANDOM,
+            fraction: float = 1.0,
+            overlap: int = 1
+    ):
+        """
+        Behaves similarly like `assign_annotators()` but instead of specify tasks_ids explicitely,
+        it gets users' IDs list and optional view ID and splits all tasks across annotators.
+        Fraction expresses the size of dataset to be assigned.
+        Parameters
+        ----------
+        users: List[int]
+            users' IDs list
+        view_id: int
+            Optional, view ID to filter tasks to assign
+        method: AssignmentSamplingMethod
+            Optional, Assignment method
+        fraction: float
+            Optional, expresses the size of dataset to be assigned
+        overlap: int
+            Optional, expresses the count of assignments for each task
+        Returns
+        -------
+        list[dict]
+            List of dicts with counter of created assignments
+        """
+        return self._assign_by_sampling(users=users,
+                                        assign_function=self.assign_annotators,
+                                        view_id=view_id,
+                                        method=method,
+                                        fraction=fraction,
+                                        overlap=overlap)
```

### Comparing `label-studio-sdk-0.0.8/label_studio_sdk/users.py` & `label-studio-sdk-0.0.9/label_studio_sdk/users.py`

 * *Files identical despite different names*

### Comparing `label-studio-sdk-0.0.8/label_studio_sdk/utils.py` & `label-studio-sdk-0.0.9/label_studio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `label-studio-sdk-0.0.8/label_studio_sdk/workspaces.py` & `label-studio-sdk-0.0.9/label_studio_sdk/workspaces.py`

 * *Files identical despite different names*

### Comparing `label-studio-sdk-0.0.8/setup.py` & `label-studio-sdk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `label-studio-sdk-0.0.8/tests/test_client.py` & `label-studio-sdk-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

