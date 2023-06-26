# Comparing `tmp/orthanc_api_client-0.9.0.tar.gz` & `tmp/orthanc_api_client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc_api_client-0.9.0.tar", last modified: Tue Feb  7 16:39:03 2023, max compression
+gzip compressed data, was "orthanc_api_client-0.9.1.tar", last modified: Thu Feb  9 14:37:32 2023, max compression
```

## Comparing `orthanc_api_client-0.9.0.tar` & `orthanc_api_client-0.9.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 16:39:03.778009 orthanc_api_client-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-02-07 16:39:03.778009 orthanc_api_client-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 16:39:03.774009 orthanc_api_client-0.9.0/orthanc_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/change.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/dicomweb_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/downloaded_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/helpers_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/modalities.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/peers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 16:39:03.778009 orthanc_api_client-0.9.0/orthanc_api_client/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/resources/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/resources/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/resources/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/resources/series_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/resources/studies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/study.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/orthanc_api_client/transfers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 16:39:03.778009 orthanc_api_client-0.9.0/orthanc_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-02-07 16:39:03.000000 orthanc_api_client-0.9.0/orthanc_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-07 16:39:03.000000 orthanc_api_client-0.9.0/orthanc_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 16:39:03.000000 orthanc_api_client-0.9.0/orthanc_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-07 16:39:03.000000 orthanc_api_client-0.9.0/orthanc_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-07 16:39:03.000000 orthanc_api_client-0.9.0/orthanc_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/release-notes.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-07 16:39:03.782009 orthanc_api_client-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 16:39:03.778009 orthanc_api_client-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    37093 2023-02-07 16:38:50.000000 orthanc_api_client-0.9.0/tests/test_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:37:32.778808 orthanc_api_client-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-02-09 14:37:32.778808 orthanc_api_client-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:37:32.774808 orthanc_api_client-0.9.1/orthanc_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/dicomweb_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/downloaded_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/helpers_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/instances_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/modalities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/peers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:37:32.778808 orthanc_api_client-0.9.1/orthanc_api_client/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/resources/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/resources/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/resources/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/resources/series_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/resources/studies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/orthanc_api_client/transfers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:37:32.774808 orthanc_api_client-0.9.1/orthanc_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-02-09 14:37:32.000000 orthanc_api_client-0.9.1/orthanc_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-09 14:37:32.000000 orthanc_api_client-0.9.1/orthanc_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:37:32.000000 orthanc_api_client-0.9.1/orthanc_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-09 14:37:32.000000 orthanc_api_client-0.9.1/orthanc_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-09 14:37:32.000000 orthanc_api_client-0.9.1/orthanc_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-09 14:37:32.778808 orthanc_api_client-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:37:32.778808 orthanc_api_client-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    39126 2023-02-09 14:37:23.000000 orthanc_api_client-0.9.1/tests/test_api_client.py
```

### Comparing `orthanc_api_client-0.9.0/LICENSE.txt` & `orthanc_api_client-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/PKG-INFO` & `orthanc_api_client-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc_api_client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python Orthanc REST API client
 Home-page: https://github.com/orthanc-team/python-orthanc-api-client
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-api-client/issues
 Project-URL: Funding, https://orthanc-team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-api-client/
@@ -35,15 +35,15 @@
 pip3 install orthanc-api-client
 ```
 
 
 Examples:
 
 ```python
-from orthanc_api_client import OrthancApiClient, ResourceType
+from orthanc_api_client import OrthancApiClient, ResourceType, InstancesSet
 import datetime
 
 orthanc_a = OrthancApiClient('http://localhost:8042', user='orthanc', pwd='orthanc')
 orthanc_b = OrthancApiClient('http://localhost:8043', user='orthanc', pwd='orthanc')
 
 if not orthanc_a.wait_started(timeout=20):
     print("Orthanc has not started after 20 sec")
@@ -139,14 +139,36 @@
 orthanc_a.transfers.send(
     target_peer='orthanc-b',
     resources_ids=[study_id],
     resource_type=ResourceType.STUDY,
     compress=True
 )
 
+# work with a snapshot of a study
+instances_set = InstancesSet.from_study(orthanc_a, study_id=study_id)
+modified_set = instances_set.modify(
+        replace_tags={
+            'InstitutionName' : 'MY'
+        },
+        keep_tags=['SOPInstanceUID', 'SeriesInstanceUID', 'StudyInstanceUID'],
+        force=True,
+        keep_source=True # we are not changing orthanc IDs -> don't delete source since it is the same as destination
+    )
+
+# send instance_set
+orthanc_a.transfers.send(  
+    target_peer='orthanc-b',
+    resources_ids=modified_set.instances_ids,
+    resource_type=ResourceType.STUDY,
+    compress=True
+)
+
+# delete after send
+modified_set.delete()
+
 ```
 
 ## helpers methods
 
 ```python
 import datetime
 from orthanc_api_client import helpers, OrthancApiClient
```

### Comparing `orthanc_api_client-0.9.0/README.md` & `orthanc_api_client-0.9.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip3 install orthanc-api-client
 ```
 
 
 Examples:
 
 ```python
-from orthanc_api_client import OrthancApiClient, ResourceType
+from orthanc_api_client import OrthancApiClient, ResourceType, InstancesSet
 import datetime
 
 orthanc_a = OrthancApiClient('http://localhost:8042', user='orthanc', pwd='orthanc')
 orthanc_b = OrthancApiClient('http://localhost:8043', user='orthanc', pwd='orthanc')
 
 if not orthanc_a.wait_started(timeout=20):
     print("Orthanc has not started after 20 sec")
@@ -114,14 +114,36 @@
 orthanc_a.transfers.send(
     target_peer='orthanc-b',
     resources_ids=[study_id],
     resource_type=ResourceType.STUDY,
     compress=True
 )
 
+# work with a snapshot of a study
+instances_set = InstancesSet.from_study(orthanc_a, study_id=study_id)
+modified_set = instances_set.modify(
+        replace_tags={
+            'InstitutionName' : 'MY'
+        },
+        keep_tags=['SOPInstanceUID', 'SeriesInstanceUID', 'StudyInstanceUID'],
+        force=True,
+        keep_source=True # we are not changing orthanc IDs -> don't delete source since it is the same as destination
+    )
+
+# send instance_set
+orthanc_a.transfers.send(  
+    target_peer='orthanc-b',
+    resources_ids=modified_set.instances_ids,
+    resource_type=ResourceType.STUDY,
+    compress=True
+)
+
+# delete after send
+modified_set.delete()
+
 ```
 
 ## helpers methods
 
 ```python
 import datetime
 from orthanc_api_client import helpers, OrthancApiClient
```

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/api_client.py` & `orthanc_api_client-0.9.1/orthanc_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/change.py` & `orthanc_api_client-0.9.1/orthanc_api_client/change.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/dicomweb_servers.py` & `orthanc_api_client-0.9.1/orthanc_api_client/dicomweb_servers.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/exceptions.py` & `orthanc_api_client-0.9.1/orthanc_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/helpers.py` & `orthanc_api_client-0.9.1/orthanc_api_client/helpers.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/helpers_internal.py` & `orthanc_api_client-0.9.1/orthanc_api_client/helpers_internal.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/http_client.py` & `orthanc_api_client-0.9.1/orthanc_api_client/http_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/instance.py` & `orthanc_api_client-0.9.1/orthanc_api_client/instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from .tags import SimplifiedTags
-import typing
+from typing import List, Optional
 
 
 class InstanceInfo:
 
     def __init__(self, json_instance: object):
         self.main_dicom_tags = SimplifiedTags(json_instance.get('MainDicomTags'))
         self.orthanc_id = json_instance.get('ID')
         self.dicom_id = self.main_dicom_tags.get('SOPInstanceUID')
         self.series_orthanc_id = json_instance.get('ParentSeries')
 
 
 class Instance:
 
-    def __init__(self, api_client, orthanc_id):
+
+    def __init__(self, api_client: 'OrthancApiClient', orthanc_id: str):
         self._api_client = api_client
         self.orthanc_id = orthanc_id
-        self._info = None
-        self._series = None
-        self._tags = None
+        self._info: Optional[InstanceInfo] = None
+        self._series: Optional['Series'] = None
+        self._tags: Optional[SimplifiedTags] = None
 
     @staticmethod
     def from_json(api_client, json_instance: object):
         instance = Instance(api_client, json_instance.get('ID'))
         instance._info = InstanceInfo(json_instance)
         return instance
 
@@ -43,21 +44,11 @@
     @property
     def series(self) -> 'Series':  # lazy creation of series object
         if self._series is None:
             self._series = self._api_client.series.get(orthanc_id=self.info.series_orthanc_id)
         return self._series
 
     @property
-    def instances(self) -> typing.List['Instance']:  # lazy creation of instances objects
-        if self._instances is None:
-            self._instances = []
-            for id in self.info.instances_orthanc_ids:
-                instance = self._api_client.instances.get(orthanc_id=self.orthanc_id)
-                self._instances.append(instance)
-
-        return self._instances
-
-    @property
     def tags(self):  # lazy loading of tags ....
         if self._tags is None:
             self._tags = self._api_client.instances.get_tags(orthanc_id=self.orthanc_id)
-        return self._tags
+        return self._tags
```

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/job.py` & `orthanc_api_client-0.9.1/orthanc_api_client/job.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/modalities.py` & `orthanc_api_client-0.9.1/orthanc_api_client/modalities.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/peers.py` & `orthanc_api_client-0.9.1/orthanc_api_client/peers.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/resources/instances.py` & `orthanc_api_client-0.9.1/orthanc_api_client/resources/instances.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/resources/jobs.py` & `orthanc_api_client-0.9.1/orthanc_api_client/resources/jobs.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/resources/resources.py` & `orthanc_api_client-0.9.1/orthanc_api_client/resources/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import requests
 import logging
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 from ..exceptions import *
 from ..helpers import to_dicom_date
 
 
 logger = logging.getLogger('api-client')
 
 
@@ -25,18 +25,21 @@
             return "Instance"
         elif self._url_segment == "patients":
             return "Patient"
 
     def get_json(self, orthanc_id: str):
         return self._api_client.get_json(f"{self._url_segment}/{orthanc_id}")
 
+    def get_json_statistics(self, orthanc_id: str):
+        return self._api_client.get_json(f"{self._url_segment}/{orthanc_id}/statistics")
+
     def get_all_ids(self) -> List[str]:
         return self._api_client.get_json(f"{self._url_segment}/")
 
-    def delete(self, orthanc_id: str = None, orthanc_ids: List[str] = None, ignore_errors: bool = False):
+    def delete(self, orthanc_id: Optional[str] = None, orthanc_ids: Optional[List[str]] = None, ignore_errors: bool = False):
 
         if orthanc_ids:
             for oi in orthanc_ids:
                 self.delete(orthanc_id=oi, ignore_errors=ignore_errors)
 
         if orthanc_id:
             logger.debug(f"deleting {self._url_segment} {orthanc_id}")
@@ -52,15 +55,15 @@
 
         for orthanc_id in all_ids:
             self.delete(orthanc_id, ignore_errors=ignore_errors)
             deleted_ids.append(orthanc_id)
         
         return deleted_ids
 
-    def set_attachment(self, orthanc_id, attachment_name, content=None, path=None, content_type=None, match_revision=None):
+    def set_attachment(self, orthanc_id: str, attachment_name: str, content: Optional[str] = None, path: Optional[str] = None, content_type: Optional[str] = None, match_revision: Optional[str] = None):
         
         if content is None and path is not None:
             with open(path, 'rb') as f:
                 content = f.read()
 
         headers = {}
 
@@ -72,40 +75,40 @@
 
         self._api_client.put(
             endpoint=f"{self._url_segment}/{orthanc_id}/attachments/{attachment_name}",
             data=content,
             headers=headers
         )
 
-    def get_attachment(self, orthanc_id, attachment_name) -> bytes:
+    def get_attachment(self, orthanc_id: str, attachment_name: str) -> bytes:
 
         content, revision = self.get_attachment_with_revision(
             orthanc_id=orthanc_id,
             attachment_name=attachment_name
         )
         return content
 
-    def get_attachment_with_revision(self, orthanc_id, attachment_name) -> Tuple[bytes, str]:
+    def get_attachment_with_revision(self, orthanc_id: str, attachment_name: str) -> Tuple[bytes, str]:
 
         headers = {}
 
         response = self._api_client.get(
             endpoint=f"{self._url_segment}/{orthanc_id}/attachments/{attachment_name}/data",
             headers=headers
         )
 
         return response.content, response.headers.get('etag')
 
-    def download_attachment(self, orthanc_id, attachment_name, path):
+    def download_attachment(self, orthanc_id: str, attachment_name: str, path: str):
         content = self.get_attachment(orthanc_id, attachment_name)
 
         with open(path, 'wb') as f:
             f.write(content)
 
-    def set_metadata(self, orthanc_id, metadata_name, content=None, path=None, match_revision=None):
+    def set_metadata(self, orthanc_id: str, metadata_name: str, content: Optional[str] = None, path: Optional[str] = None, match_revision: Optional[str] = None):
         
         if content is None and path is not None:
             with open(path, 'rb') as f:
                 content = f.read()
 
         headers = {}
 
@@ -114,38 +117,40 @@
 
         self._api_client.put(
             endpoint=f"{self._url_segment}/{orthanc_id}/metadata/{metadata_name}",
             data=content,
             headers=headers
         )
 
-    def get_metadata(self, orthanc_id, metadata_name, default_value=None) -> bytes:
+    def get_metadata(self, orthanc_id: str, metadata_name: str, default_value: Optional[str] = None) -> bytes:
 
         content, revision = self.get_metadata_with_revision(
             orthanc_id=orthanc_id,
             metadata_name=metadata_name,
             default_value=default_value
         )
 
         return content
 
-    def get_metadata_with_revision(self, orthanc_id, metadata_name, default_value=None) -> Tuple[bytes, str]:
+    def get_metadata_with_revision(self, orthanc_id: str, metadata_name: str, default_value: Optional[str] = None) -> Tuple[bytes, str]:
 
         headers = {}
 
         try:
             response = self._api_client.get(
                 endpoint=f"{self._url_segment}/{orthanc_id}/metadata/{metadata_name}",
                 headers=headers
             )
         except ResourceNotFound:
             return default_value, None
 
         return response.content, response.headers.get('etag')
 
+    def has_metadata(self, orthanc_id: str, metadata_name: str) -> bool:
+        return self.get_metadata(orthanc_id=orthanc_id, metadata_name=metadata_name, default_value=None) is not None
 
     def _anonymize(self, orthanc_id: str, replace_tags={}, keep_tags=[], delete_original=True, force=False) -> str:
         """
         anonymizes the study/series and possibly deletes the original resource (the one that has not be anonymized)
 
         Args:
             orthanc_id: the instance id to anonymize
```

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/resources/series_list.py` & `orthanc_api_client-0.9.1/orthanc_api_client/resources/series_list.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/resources/studies.py` & `orthanc_api_client-0.9.1/orthanc_api_client/resources/studies.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/tags.py` & `orthanc_api_client-0.9.1/orthanc_api_client/tags.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client/transfers.py` & `orthanc_api_client-0.9.1/orthanc_api_client/transfers.py`

 * *Files identical despite different names*

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client.egg-info/PKG-INFO` & `orthanc_api_client-0.9.1/orthanc_api_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-api-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python Orthanc REST API client
 Home-page: https://github.com/orthanc-team/python-orthanc-api-client
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-api-client/issues
 Project-URL: Funding, https://orthanc-team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-api-client/
@@ -35,15 +35,15 @@
 pip3 install orthanc-api-client
 ```
 
 
 Examples:
 
 ```python
-from orthanc_api_client import OrthancApiClient, ResourceType
+from orthanc_api_client import OrthancApiClient, ResourceType, InstancesSet
 import datetime
 
 orthanc_a = OrthancApiClient('http://localhost:8042', user='orthanc', pwd='orthanc')
 orthanc_b = OrthancApiClient('http://localhost:8043', user='orthanc', pwd='orthanc')
 
 if not orthanc_a.wait_started(timeout=20):
     print("Orthanc has not started after 20 sec")
@@ -139,14 +139,36 @@
 orthanc_a.transfers.send(
     target_peer='orthanc-b',
     resources_ids=[study_id],
     resource_type=ResourceType.STUDY,
     compress=True
 )
 
+# work with a snapshot of a study
+instances_set = InstancesSet.from_study(orthanc_a, study_id=study_id)
+modified_set = instances_set.modify(
+        replace_tags={
+            'InstitutionName' : 'MY'
+        },
+        keep_tags=['SOPInstanceUID', 'SeriesInstanceUID', 'StudyInstanceUID'],
+        force=True,
+        keep_source=True # we are not changing orthanc IDs -> don't delete source since it is the same as destination
+    )
+
+# send instance_set
+orthanc_a.transfers.send(  
+    target_peer='orthanc-b',
+    resources_ids=modified_set.instances_ids,
+    resource_type=ResourceType.STUDY,
+    compress=True
+)
+
+# delete after send
+modified_set.delete()
+
 ```
 
 ## helpers methods
 
 ```python
 import datetime
 from orthanc_api_client import helpers, OrthancApiClient
```

### Comparing `orthanc_api_client-0.9.0/orthanc_api_client.egg-info/SOURCES.txt` & `orthanc_api_client-0.9.1/orthanc_api_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 orthanc_api_client/dicomweb_servers.py
 orthanc_api_client/downloaded_instance.py
 orthanc_api_client/exceptions.py
 orthanc_api_client/helpers.py
 orthanc_api_client/helpers_internal.py
 orthanc_api_client/http_client.py
 orthanc_api_client/instance.py
+orthanc_api_client/instances_set.py
 orthanc_api_client/job.py
 orthanc_api_client/modalities.py
 orthanc_api_client/peers.py
 orthanc_api_client/series.py
 orthanc_api_client/study.py
 orthanc_api_client/tags.py
 orthanc_api_client/transfers.py
```

### Comparing `orthanc_api_client-0.9.0/release-notes.md` & `orthanc_api_client-0.9.1/release-notes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v 0.9.1
+=======
+
+- introduced `InstancesSet` class
+
 v 0.9.0
 =======
 
 - **BREAKING CHANGE:** renamed `download_study` and `download_series` into `download_instances`
 - introduced `Series`, `SeriesInfo`, `Instance` and `InstanceInfo` classes
 
 v 0.8.3
```

### Comparing `orthanc_api_client-0.9.0/setup.py` & `orthanc_api_client-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.9.0',  # Required
+    version='0.9.1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python Orthanc REST API client',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `orthanc_api_client-0.9.0/tests/test_api_client.py` & `orthanc_api_client-0.9.1/tests/test_api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import unittest
 import subprocess
 import logging
 import datetime
-from orthanc_api_client import OrthancApiClient, generate_test_dicom_file, ChangeType, ResourceType, Study, Job, JobStatus, JobType
+from orthanc_api_client import OrthancApiClient, generate_test_dicom_file, ChangeType, ResourceType, Study, Job, JobStatus, JobType, InstancesSet
 from orthanc_api_client.helpers import to_dicom_date, wait_until
 import orthanc_api_client.exceptions as api_exceptions
 import pathlib
 import asyncio
 import tempfile
 import shutil
 import os
@@ -892,11 +892,57 @@
         # download all files of the study
         study_id = self.oa.series.get_parent_study_id(series_id)
         with tempfile.TemporaryDirectory() as tempDir:
             downloaded_instances = self.oa.studies.download_instances(study_id, tempDir)
         self.assertEqual(len(instances_id), len(downloaded_instances))
 
 
+    def test_instances_set(self):
+        self.oa.delete_all_content()
+
+        # upload a partial study
+        instances_id = self.oa.upload_folder(here / 'stimuli/MR/Brain/1')
+        study_id = self.oa.instances.get_parent_study_id(instances_id[0])
+
+        instances_set = InstancesSet.from_study(api_client=self.oa, study_id=study_id)
+
+        self.assertEqual(1, len(instances_set.series_ids))
+        self.assertEqual(2, len(instances_set.instances_ids))
+        self.assertEqual(2, len(instances_set.get_instances_ids(series_id=instances_set.series_ids[0])))
+
+        # upload the second part of the study
+        instances_id = self.oa.upload_folder(here / 'stimuli/MR/Brain/2')
+        self.assertEqual(3, len(self.oa.studies.get_instances_ids(orthanc_id=study_id)))
+
+        # modify the instance set only
+        modified_set = instances_set.modify(
+            replace_tags={
+                'InstitutionName' : 'MY',
+                'PatientName': 'TOTO',
+                'PatientID': 'TEST',
+                'OtherPatientIDs': 'TEST2'
+            },
+            keep_tags=['SOPInstanceUID', 'SeriesInstanceUID', 'StudyInstanceUID'],
+            force=True,
+            keep_source=False  # we are changing the PatientID -> Orthanc IDs will change
+        )
+
+        # this should not modify the total number of instances in Orthanc
+        self.assertEqual(3, len(self.oa.instances.get_all_ids()))
+
+        # the modified set shall have the same structure as the source
+        self.assertEqual(1, len(modified_set.series_ids))
+        self.assertEqual(2, len(modified_set.instances_ids))
+        self.assertEqual(2, len(modified_set.get_instances_ids(series_id=modified_set.series_ids[0])))
+
+        # check that changes have been applied
+        self.assertEqual("TEST2", self.oa.studies.get(modified_set.study_id).patient_main_dicom_tags.get('OtherPatientIDs'))
+
+        # delete only the modified set
+        modified_set.delete()
+
+        self.assertEqual(1, len(self.oa.instances.get_all_ids()))
+
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
     unittest.main()
```

