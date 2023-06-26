# Comparing `tmp/opn_sonarqube_api-2.3.2.2952584.tar.gz` & `tmp/opn_sonarqube_api-2.3.3.3089652.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opn_sonarqube_api-2.3.2.2952584.tar", last modified: Tue May 16 14:15:32 2023, max compression
+gzip compressed data, was "dist/opn_sonarqube_api-2.3.3.3089652.tar", last modified: Mon Jun 26 07:33:16 2023, max compression
```

## Comparing `opn_sonarqube_api-2.3.2.2952584.tar` & `opn_sonarqube_api-2.3.3.3089652.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/
--rw-rw-rw-   0 root         (0) root         (0)     3862 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    18515 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonar.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/
--rw-rw-rw-   0 root         (0) root         (0)     5675 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/export_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5331 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/migrate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/activate_rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/
--rw-rw-rw-   0 root         (0) root         (0)     3294 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/rules.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/projects.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6268 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/qualityprofiles.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/components.py
--rw-rw-rw-   0 root         (0) root         (0)     9702 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/users.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7502 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/qualitygates.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/branches.py
--rw-rw-rw-   0 root         (0) root         (0)     1875 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/user_token.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5918 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:15:32.000000 opn_sonarqube_api-2.3.2.2952584/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15993 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-16 14:09:49.000000 opn_sonarqube_api-2.3.2.2952584/DESCRIPTION.rst
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-05-16 14:15:31.000000 opn_sonarqube_api-2.3.2.2952584/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15993 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/DESCRIPTION.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3862 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/activate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/export_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5331 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/migrate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18515 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonar.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/
+-rw-rw-rw-   0 root         (0) root         (0)     7787 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualitygates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     6268 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualityprofiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     9702 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1875 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/branches.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/components.py
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/projects.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/MANIFEST.in
```

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/api.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/api.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonar.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonar.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/export_rules.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/export_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/migrate_rules.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/migrate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/cmd/activate_rules.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/activate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/rules.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/projects.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/projects.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/settings.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/settings.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/qualityprofiles.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualityprofiles.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/metrics.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/metrics.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/authentication.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/authentication.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/components.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/components.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/permissions.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/permissions.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/resources.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/resources.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/qualitygates.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualitygates.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,16 +40,19 @@
                 self.destroy(existing_qg["id"])
         except:
             # QG does not exist
             True
 
         qualitygate = self.create(data["name"])
         if qualitygate is not None:
+            new_existing_qg = self.show(None, data["name"])
+            for c in new_existing_qg["conditions"]:
+                self.delete_condition(c["id"])
             for c in data['conditions']:
-                self.create_condition(qualitygate["id"], c["metric"], c["op"], c["error"])
+                self.create_condition(qualitygate["name"], c["metric"], c["op"], c["error"])
             return qualitygate
 
     def list(self):
         """
         list quality gates.
 
         :return: request response
@@ -63,20 +66,24 @@
         get quality gate details, using id or name (id is prior is both are set)
 
         :param id: id of the quality gate
         :param name: name of the quality gate
         :return: request response
         """
         # Build main data to get
-        params = {
-            'id' if id is not None else 'name': id if id is not None else name
-        }
+        #params = {
+        #    'id' if id is not None else 'name': id if id is not None else name
+        #}
+        if id is not None:
+            combined="?id="+id
+        else:
+            combined="?name="+name
 
         # Make call (might raise exception) and return
-        res = self._api._get_call(self.DETAIL_ENDPOINT, params=params)
+        res = self._api._get_call(self.DETAIL_ENDPOINT, params=combined)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def create(self, name):
         """
         create a new empty quality agte
 
         :param name: name of the quality gate
@@ -157,38 +164,38 @@
             'organization': organization
         }
 
         # Make call (might raise exception) and return
         res = self._api._get_call(self.PROJECT_ENDPOINT, params=data)
         return res if res.status_code == 204 else json.loads(res.content)
 
-    def create_condition(self, gateid, metric, op, error):
+    def create_condition(self, gatename, metric, op, error):
         """
         create a condition for a quality gate
 
-        :param gateid: id of the quality gate
+        :param gatename: name of the quality gate
         :param metric: metric of the condition
         :param op: operator of the condition
         :param error: value of the condition
         :return: request response
         """
         # Build main data to post
         data = {
-            'gateId': gateid,
+            'gateName': gatename,
             'metric': metric,
             'op': op,
             'error': error
         }
 
         # Make call (might raise exception) and return
         try:
             res = self._api._make_call('post', self.CREATE_COND_ENDPOINT, data=data)
             return res if res.status_code == 204 else json.loads(res.content)
         except ClientError:
-            print ('Error trying to create condition for quality gate %s with metric %s, op %s, and error %s.' % (gateid, metric, op, error))
+            print ('Error trying to create condition for quality gate %s with metric %s, op %s, and error %s.' % (gatename, metric, op, error))
 
     def delete_condition(self, id):
         """
         delete a condition in quality gate
 
         :param id: id of the condition gate
         :return: request response
```

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/groups.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/groups.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/branches.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/branches.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/sonarqube_api/sonarapi/user_token.py` & `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/user_token.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/PKG-INFO` & `opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: opn_sonarqube_api
-Version: 2.3.2.2952584
+Name: opn-sonarqube-api
+Version: 2.3.3.3089652
 Summary: Open SonarQube API Handler
 Home-page: UNKNOWN
 Author: open sas
 Author-email: boost-support@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
```

### Comparing `opn_sonarqube_api-2.3.2.2952584/README.rst` & `opn_sonarqube_api-2.3.3.3089652/README.rst`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/PKG-INFO` & `opn_sonarqube_api-2.3.3.3089652/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: opn-sonarqube-api
-Version: 2.3.2.2952584
+Name: opn_sonarqube_api
+Version: 2.3.3.3089652
 Summary: Open SonarQube API Handler
 Home-page: UNKNOWN
 Author: open sas
 Author-email: boost-support@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
```

### Comparing `opn_sonarqube_api-2.3.2.2952584/opn_sonarqube_api.egg-info/SOURCES.txt` & `opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/tests/test_api.py` & `opn_sonarqube_api-2.3.3.3089652/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.2.2952584/setup.py` & `opn_sonarqube_api-2.3.3.3089652/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='opn_sonarqube_api',
 
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.3.2.2952584',
+    version='2.3.3.3089652',
 
     description='Open SonarQube API Handler',
     long_description=long_description,
     author='open sas',
     author_email='boost-support@open-groupe.com',
     license='MIT',
```

