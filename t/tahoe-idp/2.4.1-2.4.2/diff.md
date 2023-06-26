# Comparing `tmp/tahoe-idp-2.4.1.tar.gz` & `tmp/tahoe-idp-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoe-idp-2.4.1.tar", last modified: Thu Jun 22 23:57:37 2023, max compression
+gzip compressed data, was "tahoe-idp-2.4.2.tar", last modified: Mon Jun 26 18:28:32 2023, max compression
```

## Comparing `tahoe-idp-2.4.1.tar` & `tahoe-idp-2.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:37.408102 tahoe-idp-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-22 23:57:37.408102 tahoe-idp-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-22 23:57:37.408102 tahoe-idp-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:37.404101 tahoe-idp-2.4.1/tahoe_idp/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/magiclink_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/magiclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/magiclink_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/magiclink_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:37.408102 tahoe-idp-2.4.1/tahoe_idp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/migrations/0002_allow_null_redirect_url.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:37.408102 tahoe-idp-2.4.1/tahoe_idp/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/settings/cms_production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/settings/common_production.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/settings/lms_production.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 23:57:25.000000 tahoe-idp-2.4.1/tahoe_idp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:57:37.404101 tahoe-idp-2.4.1/tahoe_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-22 23:57:37.000000 tahoe-idp-2.4.1/tahoe_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 23:57:37.000000 tahoe-idp-2.4.1/tahoe_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:57:37.000000 tahoe-idp-2.4.1/tahoe_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 23:57:37.000000 tahoe-idp-2.4.1/tahoe_idp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 23:57:37.000000 tahoe-idp-2.4.1/tahoe_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:32.004070 tahoe-idp-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-26 18:28:32.004070 tahoe-idp-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-26 18:28:32.004070 tahoe-idp-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:32.000070 tahoe-idp-2.4.2/tahoe_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/magiclink_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/magiclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/magiclink_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/magiclink_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:32.004070 tahoe-idp-2.4.2/tahoe_idp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/migrations/0002_allow_null_redirect_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:32.004070 tahoe-idp-2.4.2/tahoe_idp/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/settings/cms_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/settings/common_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/settings/lms_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 18:28:20.000000 tahoe-idp-2.4.2/tahoe_idp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:28:32.004070 tahoe-idp-2.4.2/tahoe_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-26 18:28:31.000000 tahoe-idp-2.4.2/tahoe_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-26 18:28:31.000000 tahoe-idp-2.4.2/tahoe_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:28:31.000000 tahoe-idp-2.4.2/tahoe_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 18:28:31.000000 tahoe-idp-2.4.2/tahoe_idp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 18:28:31.000000 tahoe-idp-2.4.2/tahoe_idp.egg-info/top_level.txt
```

### Comparing `tahoe-idp-2.4.1/LICENSE` & `tahoe-idp-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/PKG-INFO` & `tahoe-idp-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoe-idp
-Version: 2.4.1
+Version: 2.4.2
 Summary: Tahoe IdP user authentication package for Tahoe.
 Home-page: https://github.com/appsembler/tahoe-idp
 Author: Appsembler
 Author-email: ops@appsembler.com
 Project-URL: Bug Tracker, https://github.com/appsembler/tahoe-idp/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tahoe-idp-2.4.1/README.md` & `tahoe-idp-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/setup.cfg` & `tahoe-idp-2.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/setup.py` & `tahoe-idp-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/api.py` & `tahoe-idp-2.4.2/tahoe_idp/api.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/apps.py` & `tahoe-idp-2.4.2/tahoe_idp/apps.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/backend.py` & `tahoe-idp-2.4.2/tahoe_idp/backend.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/helpers.py` & `tahoe-idp-2.4.2/tahoe_idp/helpers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/magiclink_backends.py` & `tahoe-idp-2.4.2/tahoe_idp/magiclink_backends.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/magiclink_helpers.py` & `tahoe-idp-2.4.2/tahoe_idp/magiclink_helpers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/magiclink_views.py` & `tahoe-idp-2.4.2/tahoe_idp/magiclink_views.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/migrations/0001_initial.py` & `tahoe-idp-2.4.2/tahoe_idp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/models.py` & `tahoe-idp-2.4.2/tahoe_idp/models.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/permissions.py` & `tahoe-idp-2.4.2/tahoe_idp/permissions.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp/receivers.py` & `tahoe-idp-2.4.2/tahoe_idp/receivers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if kwargs['created']:
         return
 
     fields_to_sync = constants.USER_FIELDS_TO_SYNC_OPENEDX_TO_IDP
 
     user_update_dict = {}
 
-    for field in instance.fields:
+    for field in instance._meta.fields:
         if field.name in fields_to_sync.keys():
             user_update_dict[fields_to_sync[field.name]] = getattr(instance, field.name)
 
     # will raise an Exception from raise_for_status if failure code
     api.update_user(instance, {
             'user': user_update_dict
         }
```

### Comparing `tahoe-idp-2.4.1/tahoe_idp/settings/common_production.py` & `tahoe-idp-2.4.2/tahoe_idp/settings/common_production.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.1/tahoe_idp.egg-info/PKG-INFO` & `tahoe-idp-2.4.2/tahoe_idp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoe-idp
-Version: 2.4.1
+Version: 2.4.2
 Summary: Tahoe IdP user authentication package for Tahoe.
 Home-page: https://github.com/appsembler/tahoe-idp
 Author: Appsembler
 Author-email: ops@appsembler.com
 Project-URL: Bug Tracker, https://github.com/appsembler/tahoe-idp/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tahoe-idp-2.4.1/tahoe_idp.egg-info/SOURCES.txt` & `tahoe-idp-2.4.2/tahoe_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

