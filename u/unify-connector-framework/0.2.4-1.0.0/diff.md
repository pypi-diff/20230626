# Comparing `tmp/unify-connector-framework-0.2.4.tar.gz` & `tmp/unify-connector-framework-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-connector-framework-0.2.4.tar", last modified: Tue Apr 18 16:45:51 2023, max compression
+gzip compressed data, was "dist/unify-connector-framework-1.0.0.tar", last modified: Mon Jun 26 21:54:32 2023, max compression
```

## Comparing `unify-connector-framework-0.2.4.tar` & `unify-connector-framework-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unifyconnectorframework/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/connector_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/logging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17872 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/organization_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unify_connector_framework.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 21:54:32.000000 unify-connector-framework-1.0.0/unifyconnectorframework/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/connector_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17963 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/organization_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2023-06-26 21:54:26.000000 unify-connector-framework-1.0.0/unifyconnectorframework/utils.py
```

### Comparing `unify-connector-framework-0.2.4/LICENSE` & `unify-connector-framework-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.4/PKG-INFO` & `unify-connector-framework-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 0.2.4
+Version: 1.0.0
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-0.2.4/README.md` & `unify-connector-framework-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.4/setup.py` & `unify-connector-framework-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.4/unify_connector_framework.egg-info/PKG-INFO` & `unify-connector-framework-1.0.0/unify_connector_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 0.2.4
+Version: 1.0.0
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-0.2.4/unifyconnectorframework/__init__.py` & `unify-connector-framework-1.0.0/unifyconnectorframework/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 """
 Defines package information
 """
 from .organization_client import DatasetOperation, OrganizationClient
 from .connector_handler import ConnectorHandler
 from .connector import Connector
 
-__version__ = "0.2.4"
+__version__ = "1.0.0"
```

### Comparing `unify-connector-framework-0.2.4/unifyconnectorframework/connector.py` & `unify-connector-framework-1.0.0/unifyconnectorframework/connector.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.4/unifyconnectorframework/connector_handler.py` & `unify-connector-framework-1.0.0/unifyconnectorframework/connector_handler.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.4/unifyconnectorframework/logging.py` & `unify-connector-framework-1.0.0/unifyconnectorframework/logging.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.4/unifyconnectorframework/organization_client.py` & `unify-connector-framework-1.0.0/unifyconnectorframework/organization_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,19 @@
         :type dataset_id: string or dict
         :param dataset_id: Existing dataset id
         """
         dataset_id_str = self.resolve_dataset_id(dataset_id)
         list_datasets = self.list_datasets()
         existing_datasets = [dataset.get("id", {}).get('id') for dataset in list_datasets]
         if dataset_id_str is None or dataset_id_str not in existing_datasets:
-            response = self.create_dataset(name=dataset_name, dataset_csv=dataset_csv)
+            response = self.create_dataset(
+                name=dataset_name,
+                dataset_csv=dataset_csv,
+                wait_until_ready=True
+            )
             dataset_id_str = response.get("data_set_id")
         else:
             self.truncate_dataset(dataset_id=dataset_id_str)
             self.append_dataset(dataset_id=dataset_id_str, dataset_csv=dataset_csv)
             dataset_name = [x['name'] for x in list_datasets if x['id']['id']==dataset_id_str][0]
 
         return dataset_id_str, dataset_name
@@ -236,15 +240,15 @@
         :type dataset_id: string or dict
         :param dataset_id: Existing dataset id
         :type operation: Enum
         :param operation: Operation on dataset, update or append
         """
         dataset_id_str = self.resolve_dataset_id(dataset_id)
         if dataset_id_str is None:
-            dataset_id_str = self.create_dataset(dataset_name, dataset_csv)['data_set_id']
+            dataset_id_str = self.create_dataset(dataset_name, dataset_csv, True)['data_set_id']
             self.log.info('create dataset %s id %s to cluster: %s, organization: %d',
                 dataset_name, dataset_id_str, self.cluster, self.org_id)
         else:
             # validate dataset_id
             existing_datasets = [
                 dataset.get("id", {}).get('id') for dataset in self.list_datasets()
             ]
```

### Comparing `unify-connector-framework-0.2.4/unifyconnectorframework/utils.py` & `unify-connector-framework-1.0.0/unifyconnectorframework/utils.py`

 * *Files identical despite different names*

