# Comparing `tmp/workos-1.8.0.tar.gz` & `tmp/workos-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/workos-1.8.0.tar", last modified: Thu Feb 24 03:32:25 2022, max compression
+gzip compressed data, was "dist/workos-1.9.0.tar", last modified: Mon Feb 28 22:27:15 2022, max compression
```

## Comparing `workos-1.8.0.tar` & `workos-1.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:25.000000 workos-1.8.0/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1063 2022-02-24 03:32:17.000000 workos-1.8.0/LICENSE
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2267 2022-02-24 03:32:25.000000 workos-1.8.0/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1334 2022-02-24 03:32:17.000000 workos-1.8.0/README.md
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2022-02-24 03:32:25.000000 workos-1.8.0/setup.cfg
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1689 2022-02-24 03:32:17.000000 workos-1.8.0/setup.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:25.000000 workos-1.8.0/workos/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      405 2022-02-24 03:32:17.000000 workos-1.8.0/workos/__about__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      207 2022-02-24 03:32:17.000000 workos-1.8.0/workos/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     6413 2022-02-24 03:32:17.000000 workos-1.8.0/workos/audit_trail.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1554 2022-02-24 03:32:17.000000 workos-1.8.0/workos/client.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     5629 2022-02-24 03:32:17.000000 workos-1.8.0/workos/directory_sync.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1497 2022-02-24 03:32:17.000000 workos-1.8.0/workos/exceptions.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4419 2022-02-24 03:32:17.000000 workos-1.8.0/workos/organizations.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2620 2022-02-24 03:32:17.000000 workos-1.8.0/workos/passwordless.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1540 2022-02-24 03:32:17.000000 workos-1.8.0/workos/portal.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:25.000000 workos-1.8.0/workos/resources/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:17.000000 workos-1.8.0/workos/resources/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1024 2022-02-24 03:32:17.000000 workos-1.8.0/workos/resources/base.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1101 2022-02-24 03:32:17.000000 workos-1.8.0/workos/resources/event.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      357 2022-02-24 03:32:17.000000 workos-1.8.0/workos/resources/event_action.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1412 2022-02-24 03:32:17.000000 workos-1.8.0/workos/resources/sso.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8101 2022-02-24 03:32:17.000000 workos-1.8.0/workos/sso.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:25.000000 workos-1.8.0/workos/utils/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:17.000000 workos-1.8.0/workos/utils/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      462 2022-02-24 03:32:17.000000 workos-1.8.0/workos/utils/connection_types.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2963 2022-02-24 03:32:17.000000 workos-1.8.0/workos/utils/request.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1301 2022-02-24 03:32:17.000000 workos-1.8.0/workos/utils/validation.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3093 2022-02-24 03:32:17.000000 workos-1.8.0/workos/webhooks.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-24 03:32:25.000000 workos-1.8.0/workos.egg-info/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2267 2022-02-24 03:32:25.000000 workos-1.8.0/workos.egg-info/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      671 2022-02-24 03:32:25.000000 workos-1.8.0/workos.egg-info/SOURCES.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2022-02-24 03:32:25.000000 workos-1.8.0/workos.egg-info/dependency_links.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2022-02-24 03:32:24.000000 workos-1.8.0/workos.egg-info/not-zip-safe
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      135 2022-02-24 03:32:25.000000 workos-1.8.0/workos.egg-info/requires.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        7 2022-02-24 03:32:25.000000 workos-1.8.0/workos.egg-info/top_level.txt
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:15.000000 workos-1.9.0/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1063 2022-02-28 22:27:06.000000 workos-1.9.0/LICENSE
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2267 2022-02-28 22:27:15.000000 workos-1.9.0/PKG-INFO
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1334 2022-02-28 22:27:06.000000 workos-1.9.0/README.md
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2022-02-28 22:27:15.000000 workos-1.9.0/setup.cfg
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1689 2022-02-28 22:27:06.000000 workos-1.9.0/setup.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:15.000000 workos-1.9.0/workos/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      405 2022-02-28 22:27:06.000000 workos-1.9.0/workos/__about__.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      207 2022-02-28 22:27:06.000000 workos-1.9.0/workos/__init__.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     6413 2022-02-28 22:27:06.000000 workos-1.9.0/workos/audit_trail.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1554 2022-02-28 22:27:06.000000 workos-1.9.0/workos/client.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     5801 2022-02-28 22:27:06.000000 workos-1.9.0/workos/directory_sync.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1497 2022-02-28 22:27:06.000000 workos-1.9.0/workos/exceptions.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4419 2022-02-28 22:27:06.000000 workos-1.9.0/workos/organizations.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2620 2022-02-28 22:27:06.000000 workos-1.9.0/workos/passwordless.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1540 2022-02-28 22:27:06.000000 workos-1.9.0/workos/portal.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:15.000000 workos-1.9.0/workos/resources/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:06.000000 workos-1.9.0/workos/resources/__init__.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1024 2022-02-28 22:27:06.000000 workos-1.9.0/workos/resources/base.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1101 2022-02-28 22:27:06.000000 workos-1.9.0/workos/resources/event.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      357 2022-02-28 22:27:06.000000 workos-1.9.0/workos/resources/event_action.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1412 2022-02-28 22:27:06.000000 workos-1.9.0/workos/resources/sso.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8101 2022-02-28 22:27:06.000000 workos-1.9.0/workos/sso.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:15.000000 workos-1.9.0/workos/utils/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:06.000000 workos-1.9.0/workos/utils/__init__.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      462 2022-02-28 22:27:06.000000 workos-1.9.0/workos/utils/connection_types.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2963 2022-02-28 22:27:06.000000 workos-1.9.0/workos/utils/request.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1301 2022-02-28 22:27:06.000000 workos-1.9.0/workos/utils/validation.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3093 2022-02-28 22:27:06.000000 workos-1.9.0/workos/webhooks.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-02-28 22:27:15.000000 workos-1.9.0/workos.egg-info/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2267 2022-02-28 22:27:15.000000 workos-1.9.0/workos.egg-info/PKG-INFO
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      671 2022-02-28 22:27:15.000000 workos-1.9.0/workos.egg-info/SOURCES.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2022-02-28 22:27:15.000000 workos-1.9.0/workos.egg-info/dependency_links.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2022-02-28 22:27:14.000000 workos-1.9.0/workos.egg-info/not-zip-safe
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      135 2022-02-28 22:27:15.000000 workos-1.9.0/workos.egg-info/requires.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        7 2022-02-28 22:27:15.000000 workos-1.9.0/workos.egg-info/top_level.txt
```

### Comparing `workos-1.8.0/LICENSE` & `workos-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/PKG-INFO` & `workos-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 1.8.0
+Version: 1.9.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-1.8.0/README.md` & `workos-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/setup.py` & `workos-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/audit_trail.py` & `workos-1.9.0/workos/audit_trail.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/client.py` & `workos-1.9.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/directory_sync.py` & `workos-1.9.0/workos/directory_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,30 +107,38 @@
         return self.request_helper.request(
             "directory_groups/{group}".format(group=group),
             method=REQUEST_METHOD_GET,
             token=workos.api_key,
         )
 
     def list_directories(
-        self, domain=None, search=None, limit=RESPONSE_LIMIT, before=None, after=None
+        self,
+        domain=None,
+        search=None,
+        limit=RESPONSE_LIMIT,
+        before=None,
+        after=None,
+        organization=None,
     ):
         """Gets details for existing Directories.
 
         Args:
             domain (str): Domain of a Directory. (Optional)
+            organization: ID of an Organization (Optional)
             search (str): Searchable text for a Directory. (Optional)
             limit (int): Maximum number of records to return. (Optional)
             before (str): Pagination cursor to receive records before a provided Directory ID. (Optional)
             after (str): Pagination cursor to receive records after a provided Directory ID. (Optional)
 
         Returns:
             dict: Directories response from WorkOS.
         """
         params = {
             "domain": domain,
+            "organization_id": organization,
             "search": search,
             "limit": limit,
             "before": before,
             "after": after,
         }
         return self.request_helper.request(
             "directories",
```

### Comparing `workos-1.8.0/workos/exceptions.py` & `workos-1.9.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/organizations.py` & `workos-1.9.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/passwordless.py` & `workos-1.9.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/portal.py` & `workos-1.9.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/resources/base.py` & `workos-1.9.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/resources/event.py` & `workos-1.9.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/resources/sso.py` & `workos-1.9.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/sso.py` & `workos-1.9.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/utils/request.py` & `workos-1.9.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/utils/validation.py` & `workos-1.9.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos/webhooks.py` & `workos-1.9.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-1.8.0/workos.egg-info/PKG-INFO` & `workos-1.9.0/workos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 1.8.0
+Version: 1.9.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-1.8.0/workos.egg-info/SOURCES.txt` & `workos-1.9.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

