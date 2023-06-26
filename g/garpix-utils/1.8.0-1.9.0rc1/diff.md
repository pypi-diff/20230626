# Comparing `tmp/garpix_utils-1.8.0.tar.gz` & `tmp/garpix_utils-1.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_utils-1.8.0.tar", last modified: Wed Feb  1 13:35:53 2023, max compression
+gzip compressed data, was "garpix_utils-1.9.0rc1.tar", last modified: Mon Jun 26 12:27:27 2023, max compression
```

## Comparing `garpix_utils-1.8.0.tar` & `garpix_utils-1.9.0rc1.tar`

### file list

```diff
@@ -1,54 +1,106 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.634015 garpix_utils-1.8.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       32 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10500 2023-02-01 13:35:53.633843 garpix_utils-1.8.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.630214 garpix_utils-1.8.0/garpix_utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       32 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9934 2022-11-30 09:52:10.000000 garpix_utils-1.8.0/garpix_utils/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       59 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.631039 garpix_utils-1.8.0/garpix_utils/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       61 2022-10-07 15:35:43.000000 garpix_utils-1.8.0/garpix_utils/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      611 2022-10-07 15:35:43.000000 garpix_utils-1.8.0/garpix_utils/admin/site_configuration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      131 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.631331 garpix_utils-1.8.0/garpix_utils/file/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       76 2022-11-30 09:52:10.000000 garpix_utils-1.8.0/garpix_utils/file/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      489 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/file/file_field.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      652 2022-11-30 09:52:10.000000 garpix_utils-1.8.0/garpix_utils/file/filepath.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.632100 garpix_utils-1.8.0/garpix_utils/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-02-01 13:35:31.000000 garpix_utils-1.8.0/garpix_utils/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      157 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/managers/active_manager.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      194 2023-02-01 13:35:31.000000 garpix_utils-1.8.0/garpix_utils/managers/active_on_site_manager.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      178 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/managers/available_manager.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      140 2022-10-07 14:31:15.000000 garpix_utils-1.8.0/garpix_utils/managers/current_site_manager.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      195 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/managers/polymorphic_active_manager.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      216 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/managers/polymorphic_available_manager.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      562 2022-10-07 14:31:15.000000 garpix_utils-1.8.0/garpix_utils/managers/polymorphic_current_site_manager.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.633076 garpix_utils-1.8.0/garpix_utils/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      389 2022-10-07 15:35:43.000000 garpix_utils-1.8.0/garpix_utils/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/active_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      519 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/admin_delete_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      268 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/available_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      377 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/delete_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/empty_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/polymorphic_active_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      392 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/models/polymorphic_available_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1503 2022-10-07 15:35:43.000000 garpix_utils-1.8.0/garpix_utils/models/site_configuration.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.633282 garpix_utils-1.8.0/garpix_utils/paginator/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       39 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/paginator/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1445 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/paginator/paginator.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1174 2023-02-01 13:35:31.000000 garpix_utils-1.8.0/garpix_utils/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.633381 garpix_utils-1.8.0/garpix_utils/signature/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3860 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/signature/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.633481 garpix_utils-1.8.0/garpix_utils/string/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      336 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/string/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.633668 garpix_utils-1.8.0/garpix_utils/templatetags/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       45 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/templatetags/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      418 2022-06-23 10:15:14.000000 garpix_utils-1.8.0/garpix_utils/templatetags/url_replace.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-02-01 13:35:53.630828 garpix_utils-1.8.0/garpix_utils.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10500 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/garpix_utils.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1468 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/garpix_utils.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/garpix_utils.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/garpix_utils.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       81 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/garpix_utils.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       13 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/garpix_utils.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-02-01 13:35:53.634051 garpix_utils-1.8.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1174 2023-02-01 13:35:53.000000 garpix_utils-1.8.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.019309 garpix_utils-1.9.0rc1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       32 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10503 2023-06-26 12:27:27.019013 garpix_utils-1.9.0rc1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.002325 garpix_utils-1.9.0rc1/garpix_utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       32 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9934 2022-11-30 09:52:10.000000 garpix_utils-1.9.0rc1/garpix_utils/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       59 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.003060 garpix_utils-1.9.0rc1/garpix_utils/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      225 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.003269 garpix_utils-1.9.0rc1/garpix_utils/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       61 2022-10-07 15:35:43.000000 garpix_utils-1.9.0rc1/garpix_utils/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.003568 garpix_utils-1.9.0rc1/garpix_utils/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      244 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1231 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/admin/__pycache__/site_configuration.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      611 2022-10-07 15:35:43.000000 garpix_utils-1.9.0rc1/garpix_utils/admin/site_configuration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      131 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.003931 garpix_utils-1.9.0rc1/garpix_utils/file/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      107 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/file/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.004488 garpix_utils-1.9.0rc1/garpix_utils/file/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      317 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/file/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2153 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/file/__pycache__/file_field.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      804 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/file/__pycache__/filepath.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1594 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/file/file_field.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      652 2022-11-30 09:52:10.000000 garpix_utils-1.9.0rc1/garpix_utils/file/filepath.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.009477 garpix_utils-1.9.0rc1/garpix_utils/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-02-01 13:35:31.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.013423 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      659 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      601 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/active_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      635 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/active_on_site_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      625 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/available_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      452 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/current_site_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      647 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/polymorphic_active_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      671 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/polymorphic_available_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      965 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/__pycache__/polymorphic_current_site_manager.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      157 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/active_manager.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      194 2023-02-01 13:35:31.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/active_on_site_manager.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      178 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/available_manager.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      140 2022-10-07 14:31:15.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/current_site_manager.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      195 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/polymorphic_active_manager.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      216 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/polymorphic_available_manager.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      562 2022-10-07 14:31:15.000000 garpix_utils-1.9.0rc1/garpix_utils/managers/polymorphic_current_site_manager.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.014570 garpix_utils-1.9.0rc1/garpix_utils/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      436 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.015645 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      700 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      731 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/active_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1053 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/admin_delete_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/available_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1006 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/delete_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      540 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/empty_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      847 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/polymorphic_active_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      837 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/polymorphic_available_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      905 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/secret_file_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2496 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/models/__pycache__/site_configuration.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/active_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      519 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/admin_delete_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      268 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/available_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      377 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/delete_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/empty_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/polymorphic_active_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      392 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/models/polymorphic_available_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      433 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/models/secret_file_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1503 2022-10-07 15:35:43.000000 garpix_utils-1.9.0rc1/garpix_utils/models/site_configuration.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.015844 garpix_utils-1.9.0rc1/garpix_utils/paginator/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       39 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/paginator/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.016057 garpix_utils-1.9.0rc1/garpix_utils/paginator/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/paginator/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1680 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/paginator/__pycache__/paginator.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1445 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/paginator/paginator.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.016258 garpix_utils-1.9.0rc1/garpix_utils/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/serializers/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.016480 garpix_utils-1.9.0rc1/garpix_utils/serializers/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      257 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/serializers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      830 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/serializers/__pycache__/secret_file_serializer_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/serializers/secret_file_serializer_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1218 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.016595 garpix_utils-1.9.0rc1/garpix_utils/signature/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3860 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/signature/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.016744 garpix_utils-1.9.0rc1/garpix_utils/signature/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4031 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/signature/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.016892 garpix_utils-1.9.0rc1/garpix_utils/string/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      662 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/string/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.017054 garpix_utils-1.9.0rc1/garpix_utils/string/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1402 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/string/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.017328 garpix_utils-1.9.0rc1/garpix_utils/templatetags/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       45 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/templatetags/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.017618 garpix_utils-1.9.0rc1/garpix_utils/templatetags/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      212 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      653 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/templatetags/__pycache__/url_replace.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      418 2022-06-23 10:15:14.000000 garpix_utils-1.9.0rc1/garpix_utils/templatetags/url_replace.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.017871 garpix_utils-1.9.0rc1/garpix_utils/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       56 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/views/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.018150 garpix_utils-1.9.0rc1/garpix_utils/views/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/views/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1041 2023-06-26 09:51:23.000000 garpix_utils-1.9.0rc1/garpix_utils/views/__pycache__/secret_file_view_mixin.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      592 2023-06-26 12:27:08.000000 garpix_utils-1.9.0rc1/garpix_utils/views/secret_file_view_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:27:27.002953 garpix_utils-1.9.0rc1/garpix_utils.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10503 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/garpix_utils.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3849 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/garpix_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/garpix_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/garpix_utils.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      109 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/garpix_utils.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       13 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/garpix_utils.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-26 12:27:27.020232 garpix_utils-1.9.0rc1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1218 2023-06-26 12:27:26.000000 garpix_utils-1.9.0rc1/setup.py
```

### Comparing `garpix_utils-1.8.0/PKG-INFO` & `garpix_utils-1.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_utils
-Version: 1.8.0
+Version: 1.9.0rc1
 Home-page: https://github.com/garpixcms/garpix_utils
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_utils-1.8.0/garpix_utils/README.md` & `garpix_utils-1.9.0rc1/garpix_utils/README.md`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/admin/site_configuration.py` & `garpix_utils-1.9.0rc1/garpix_utils/admin/site_configuration.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/file/filepath.py` & `garpix_utils-1.9.0rc1/garpix_utils/file/filepath.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/managers/polymorphic_current_site_manager.py` & `garpix_utils-1.9.0rc1/garpix_utils/managers/polymorphic_current_site_manager.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/models/admin_delete_mixin.py` & `garpix_utils-1.9.0rc1/garpix_utils/models/admin_delete_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/models/site_configuration.py` & `garpix_utils-1.9.0rc1/garpix_utils/models/site_configuration.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/paginator/paginator.py` & `garpix_utils-1.9.0rc1/garpix_utils/paginator/paginator.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils/setup.py` & `garpix_utils-1.9.0rc1/garpix_utils/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_utils')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_utils',
-    version='1.8.0',
+    version='1.9.0-rc1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_utils',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -30,9 +30,10 @@
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'django-uuslug >= 1.2.0',
         'django-polymorphic-tree-for-garpix-page >= 2.0.1',
+        'djangorestframework >= 3.14.0'
     ],
 )
```

### Comparing `garpix_utils-1.8.0/garpix_utils/signature/__init__.py` & `garpix_utils-1.9.0rc1/garpix_utils/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_utils-1.8.0/garpix_utils.egg-info/PKG-INFO` & `garpix_utils-1.9.0rc1/garpix_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-utils
-Version: 1.8.0
+Version: 1.9.0rc1
 Home-page: https://github.com/garpixcms/garpix_utils
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_utils-1.8.0/setup.py` & `garpix_utils-1.9.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_utils')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_utils',
-    version='1.8.0',
+    version='1.9.0-rc1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_utils',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -30,9 +30,10 @@
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'django-uuslug >= 1.2.0',
         'django-polymorphic-tree-for-garpix-page >= 2.0.1',
+        'djangorestframework >= 3.14.0'
     ],
 )
```

