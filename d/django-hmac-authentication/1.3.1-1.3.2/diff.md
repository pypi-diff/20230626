# Comparing `tmp/django_hmac_authentication-1.3.1.tar.gz` & `tmp/django_hmac_authentication-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.3.1.tar", last modified: Wed Jun 21 22:57:41 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.3.2.tar", last modified: Mon Jun 26 08:56:03 2023, max compression
```

## Comparing `django_hmac_authentication-1.3.1.tar` & `django_hmac_authentication-1.3.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5810 2023-06-13 03:07:01.000000 django_hmac_authentication-1.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-21 22:51:16.000000 django_hmac_authentication-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.190257 django_hmac_authentication-1.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.194257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-21 22:51:16.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/aes.py
--rw-rw-rw-   0 root         (0) root         (0)     4485 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/client_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 22:57:04.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 22:57:04.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 22:57:04.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/padding.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1232 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5810 2023-06-13 03:07:01.000000 django_hmac_authentication-1.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-26 08:49:07.000000 django_hmac_authentication-1.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.982444 django_hmac_authentication-1.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.986444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-26 08:49:07.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-26 08:22:01.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2023-06-26 08:43:45.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/client_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 08:55:25.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 08:55:25.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 08:55:25.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:56:03.990444 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-26 08:56:03.000000 django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/top_level.txt
```

### Comparing `django_hmac_authentication-1.3.1/LICENSE` & `django_hmac_authentication-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/PKG-INFO` & `django_hmac_authentication-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 1.3.1
+Version: 1.3.2
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-1.3.1/README.md` & `django_hmac_authentication-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/pyproject.toml` & `django_hmac_authentication-1.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["django_hmac_authentication*"]
 namespaces = false
 
 [project]
 name = "django_hmac_authentication"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hmac-authentication
-Version: 1.3.1
+Version: 1.3.2
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.3.2/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 src/django_hmac_authentication/__init__.py
 src/django_hmac_authentication/admin.py
 src/django_hmac_authentication/aes.py
+src/django_hmac_authentication/apps.py
 src/django_hmac_authentication/authentication.py
+src/django_hmac_authentication/checks.py
 src/django_hmac_authentication/client_utils.py
 src/django_hmac_authentication/exceptions.py
 src/django_hmac_authentication/models.py
 src/django_hmac_authentication/padding.py
 src/django_hmac_authentication/serializers.py
 src/django_hmac_authentication/server_utils.py
 src/django_hmac_authentication/views.py
```

