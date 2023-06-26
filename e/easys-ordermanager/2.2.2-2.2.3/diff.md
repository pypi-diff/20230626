# Comparing `tmp/easys-ordermanager-2.2.2.tar.gz` & `tmp/easys-ordermanager-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easys-ordermanager-2.2.2.tar", last modified: Thu Jun  1 13:56:39 2023, max compression
+gzip compressed data, was "easys-ordermanager-2.2.3.tar", last modified: Mon Jun 26 13:10:30 2023, max compression
```

## Comparing `easys-ordermanager-2.2.2.tar` & `easys-ordermanager-2.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/
--rw-r--r--   0 root         (0) root         (0)    12547 2023-06-01 13:56:04.000000 easys-ordermanager-2.2.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     9612 2023-06-01 13:56:04.000000 easys-ordermanager-2.2.2/CHANGELOG_SERIALIZER.md
--rw-r--r--   0 root         (0) root         (0)    34940 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22903 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-01 13:56:04.000000 easys-ordermanager-2.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/management/commands/i18n.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/tests/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/v1/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/tests/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/v2/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/dev/tests/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/dev/tests/v3/test_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/easys_ordermanager/
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-01 13:56:04.000000 easys-ordermanager-2.2.2/easys_ordermanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/easys_ordermanager/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-01 13:56:39.000000 easys-ordermanager-2.2.2/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      829 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/easys_ordermanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.140297 easys-ordermanager-2.2.2/easys_ordermanager/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/easys_ordermanager/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    13144 2023-06-01 13:56:04.000000 easys-ordermanager-2.2.2/easys_ordermanager/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/easys_ordermanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93490 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/v1/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/easys_ordermanager/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93587 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/v2/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/easys_ordermanager/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94726 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/v3/serializer.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-06-01 12:38:49.000000 easys-ordermanager-2.2.2/easys_ordermanager/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/easys_ordermanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22903 2023-06-01 13:56:39.000000 easys-ordermanager-2.2.2/easys_ordermanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-06-01 13:56:39.000000 easys-ordermanager-2.2.2/easys_ordermanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:56:39.000000 easys-ordermanager-2.2.2/easys_ordermanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-01 13:56:39.000000 easys-ordermanager-2.2.2/easys_ordermanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 13:56:39.000000 easys-ordermanager-2.2.2/easys_ordermanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-01 13:56:39.144297 easys-ordermanager-2.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-01 13:56:04.000000 easys-ordermanager-2.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.103213 easys-ordermanager-2.2.3/
+-rw-r--r--   0 root         (0) root         (0)    12623 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     9696 2023-06-26 10:10:47.000000 easys-ordermanager-2.2.3/CHANGELOG_SERIALIZER.md
+-rw-r--r--   0 root         (0) root         (0)    34940 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23063 2023-06-26 13:10:30.103213 easys-ordermanager-2.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/management/commands/i18n.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/tests/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/v1/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/tests/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/v2/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/dev/tests/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/dev/tests/v3/test_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/easys_ordermanager/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-26 10:09:38.000000 easys-ordermanager-2.2.3/easys_ordermanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/easys_ordermanager/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-26 13:10:29.000000 easys-ordermanager-2.2.3/easys_ordermanager/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      829 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/easys_ordermanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/easys_ordermanager/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/easys_ordermanager/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    13144 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.103213 easys-ordermanager-2.2.3/easys_ordermanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93490 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/v1/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.103213 easys-ordermanager-2.2.3/easys_ordermanager/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93587 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/v2/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.103213 easys-ordermanager-2.2.3/easys_ordermanager/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94874 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/v3/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/easys_ordermanager/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:10:30.099213 easys-ordermanager-2.2.3/easys_ordermanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23063 2023-06-26 13:10:30.000000 easys-ordermanager-2.2.3/easys_ordermanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-26 13:10:30.000000 easys-ordermanager-2.2.3/easys_ordermanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 13:10:30.000000 easys-ordermanager-2.2.3/easys_ordermanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-26 13:10:30.000000 easys-ordermanager-2.2.3/easys_ordermanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-26 13:10:30.000000 easys-ordermanager-2.2.3/easys_ordermanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-26 13:10:30.103213 easys-ordermanager-2.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-26 07:53:45.000000 easys-ordermanager-2.2.3/setup.py
```

### Comparing `easys-ordermanager-2.2.2/CHANGELOG.md` & `easys-ordermanager-2.2.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## 2.2.3 (2023-06-26)
+* Updates to Serializer v3, see serializer changelog
+
 ## 2.2.2 (2023-06-01)
 * Updates to Serializer v3, see serializer changelog
 
 ## 2.2.1 (2023-05-30)
 * Updated wording on translation of Domain choices field.
 
 ## 2.2.0 (2023-05-23)
```

### Comparing `easys-ordermanager-2.2.2/CHANGELOG_SERIALIZER.md` & `easys-ordermanager-2.2.3/CHANGELOG_SERIALIZER.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Serializer changes
 
+## 2.2.3
+
+### v3
+
+#### `OrderLineWebsiteSerializer`
+* Added field `internal_area`.
+
 ## 2.2.2
 
 ### v3
 
 #### `OrderLineEmailSerializer`
 * Renamed field `included_accounts` to `included_addresses`.
 * Renamed field `additional_accounts` to `additional_addresses`.
```

### Comparing `easys-ordermanager-2.2.2/LICENSE.md` & `easys-ordermanager-2.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/PKG-INFO` & `easys-ordermanager-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.2.2
+Version: 2.2.3
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -26,14 +26,17 @@
 ### Django 4.2
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.2.3 (2023-06-26)
+* Updates to Serializer v3, see serializer changelog
+
 ## 2.2.2 (2023-06-01)
 * Updates to Serializer v3, see serializer changelog
 
 ## 2.2.1 (2023-05-30)
 * Updated wording on translation of Domain choices field.
 
 ## 2.2.0 (2023-05-23)
@@ -436,14 +439,21 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.2.3
+
+### v3
+
+#### `OrderLineWebsiteSerializer`
+* Added field `internal_area`.
+
 ## 2.2.2
 
 ### v3
 
 #### `OrderLineEmailSerializer`
 * Renamed field `included_accounts` to `included_addresses`.
 * Renamed field `additional_accounts` to `additional_addresses`.
```

### Comparing `easys-ordermanager-2.2.2/dev/management/commands/i18n.py` & `easys-ordermanager-2.2.3/dev/management/commands/i18n.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/dev/tests/v3/test_serializer.py` & `easys-ordermanager-2.2.3/dev/tests/v3/test_serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/__pycache__/__init__.cpython-311.pyc` & `easys-ordermanager-2.2.3/easys_ordermanager/__pycache__/__init__.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x74a37864 (Thu Jun  1 13:56:04 2023 UTC)
+moddate:  0xe2639964 (Mon Jun 26 10:09:38 2023 UTC)
 files sz: 300
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code
@@ -13,15 +13,15 @@
    
      1           2 LOAD_CONST               0 ('easys-ordermanager')
                  4 STORE_NAME               0 (__title__)
    
      2           6 LOAD_CONST               1 ('API definition of RH order manager for EasyS')
                  8 STORE_NAME               1 (__description__)
    
-     3          10 LOAD_CONST               2 ('2.2.2')
+     3          10 LOAD_CONST               2 ('2.2.3')
                 12 STORE_NAME               2 (__version__)
    
      4          14 LOAD_CONST               3 ('https://gitlab.herocentral.de/development/easys-ordermanager')
                 16 STORE_NAME               3 (__url__)
    
      5          18 LOAD_CONST               4 ('RegioHelden developers')
                 20 STORE_NAME               4 (__author__)
@@ -32,15 +32,15 @@
      7          26 LOAD_CONST               6 ('GPL 3')
                 28 STORE_NAME               6 (__license__)
                 30 LOAD_CONST               7 (None)
                 32 RETURN_VALUE
    consts
       'easys-ordermanager'
       'API definition of RH order manager for EasyS'
-      '2.2.2'
+      '2.2.3'
       'https://gitlab.herocentral.de/development/easys-ordermanager'
       'RegioHelden developers'
       'opensource@regiohelden.de'
       'GPL 3'
       None
    names      ('__title__', '__description__', '__version__', '__url__', '__author__', '__author_email__', '__license__')
    varnames   ()
```

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/fields.py` & `easys-ordermanager-2.2.3/easys_ordermanager/fields.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/locale/de/LC_MESSAGES/django.po` & `easys-ordermanager-2.2.3/easys_ordermanager/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/v1/serializer.py` & `easys-ordermanager-2.2.3/easys_ordermanager/v1/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/v2/serializer.py` & `easys-ordermanager-2.2.3/easys_ordermanager/v2/serializer.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/v3/serializer.py` & `easys-ordermanager-2.2.3/easys_ordermanager/v3/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2019,14 +2019,20 @@
     """
     textual description of wishes and requirements for the logo
 
     """
     logo_description = serializers.CharField(max_length=1000, allow_blank=True, required=False)
 
     """
+    should the user internal area be made available for the customer?
+
+    """
+    internal_area = serializers.BooleanField(default=False)
+
+    """
     website design choice between minimalistic and embellished
 
     """
     design_preference_minimalistic_embellished = serializers.ChoiceField(
         choices=WEBSITE_DESIGN_PREFERENCE_MINIMALISTIC_EMBELLISHED, allow_null=True, required=False
     )
```

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager/validators.py` & `easys-ordermanager-2.2.3/easys_ordermanager/validators.py`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager.egg-info/PKG-INFO` & `easys-ordermanager-2.2.3/easys_ordermanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easys-ordermanager
-Version: 2.2.2
+Version: 2.2.3
 Summary: API definition of RH order manager for EasyS
 Home-page: https://gitlab.herocentral.de/development/easys-ordermanager
 Download-URL: 
 Author: RegioHelden developers
 Author-email: opensource@regiohelden.de
 License: GPL 3
 Description-Content-Type: text/markdown
@@ -26,14 +26,17 @@
 ### Django 4.2
 
 DRF 3.14 or newer
 
 
 # Changelog
 
+## 2.2.3 (2023-06-26)
+* Updates to Serializer v3, see serializer changelog
+
 ## 2.2.2 (2023-06-01)
 * Updates to Serializer v3, see serializer changelog
 
 ## 2.2.1 (2023-05-30)
 * Updated wording on translation of Domain choices field.
 
 ## 2.2.0 (2023-05-23)
@@ -436,14 +439,21 @@
 ## 1.0.0 (2019-06-24)
 
 * Initial release
 
 
 # Serializer changes
 
+## 2.2.3
+
+### v3
+
+#### `OrderLineWebsiteSerializer`
+* Added field `internal_area`.
+
 ## 2.2.2
 
 ### v3
 
 #### `OrderLineEmailSerializer`
 * Renamed field `included_accounts` to `included_addresses`.
 * Renamed field `additional_accounts` to `additional_addresses`.
```

### Comparing `easys-ordermanager-2.2.2/easys_ordermanager.egg-info/SOURCES.txt` & `easys-ordermanager-2.2.3/easys_ordermanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easys-ordermanager-2.2.2/setup.py` & `easys-ordermanager-2.2.3/setup.py`

 * *Files identical despite different names*

