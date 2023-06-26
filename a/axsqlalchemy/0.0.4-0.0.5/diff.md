# Comparing `tmp/axsqlalchemy-0.0.4.tar.gz` & `tmp/axsqlalchemy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axsqlalchemy-0.0.4.tar", last modified: Mon Jun 26 09:04:42 2023, max compression
+gzip compressed data, was "axsqlalchemy-0.0.5.tar", last modified: Mon Jun 26 09:08:17 2023, max compression
```

## Comparing `axsqlalchemy-0.0.4.tar` & `axsqlalchemy-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:04:42.321495 axsqlalchemy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 09:04:42.321495 axsqlalchemy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:04:42.321495 axsqlalchemy-0.0.4/axsqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/repository.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/uow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:04:42.321495 axsqlalchemy-0.0.4/axsqlalchemy/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/axsqlalchemy/utils/creation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:04:42.321495 axsqlalchemy-0.0.4/axsqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 09:04:42.000000 axsqlalchemy-0.0.4/axsqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-26 09:04:42.000000 axsqlalchemy-0.0.4/axsqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:04:42.000000 axsqlalchemy-0.0.4/axsqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 09:04:42.000000 axsqlalchemy-0.0.4/axsqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 09:04:42.000000 axsqlalchemy-0.0.4/axsqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:04:42.321495 axsqlalchemy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-26 09:04:15.000000 axsqlalchemy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/axsqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/repository.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/uow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/axsqlalchemy/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/utils/creation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/setup.py
```

### Comparing `axsqlalchemy-0.0.4/axsqlalchemy/model.py` & `axsqlalchemy-0.0.5/axsqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.4/axsqlalchemy/repository.py` & `axsqlalchemy-0.0.5/axsqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.4/axsqlalchemy/settings.py` & `axsqlalchemy-0.0.5/axsqlalchemy/settings.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.4/axsqlalchemy/uow.py` & `axsqlalchemy-0.0.5/axsqlalchemy/uow.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.4/axsqlalchemy/utils/creation.py` & `axsqlalchemy-0.0.5/axsqlalchemy/utils/creation.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.4/setup.py` & `axsqlalchemy-0.0.5/setup.py`

 * *Files identical despite different names*

