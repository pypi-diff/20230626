# Comparing `tmp/axsqlalchemy-0.0.1.tar.gz` & `tmp/axsqlalchemy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axsqlalchemy-0.0.1.tar", last modified: Mon Jun 26 07:00:01 2023, max compression
+gzip compressed data, was "axsqlalchemy-0.0.3.tar", last modified: Mon Jun 26 07:20:25 2023, max compression
```

## Comparing `axsqlalchemy-0.0.1.tar` & `axsqlalchemy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:01.662894 axsqlalchemy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 07:00:01.662894 axsqlalchemy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:01.658894 axsqlalchemy-0.0.1/axsqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/axsqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/axsqlalchemy/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/axsqlalchemy/repository.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/axsqlalchemy/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/axsqlalchemy/uow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:01.662894 axsqlalchemy-0.0.1/axsqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 07:00:01.000000 axsqlalchemy-0.0.1/axsqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-26 07:00:01.000000 axsqlalchemy-0.0.1/axsqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:00:01.000000 axsqlalchemy-0.0.1/axsqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 07:00:01.000000 axsqlalchemy-0.0.1/axsqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 07:00:01.000000 axsqlalchemy-0.0.1/axsqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 07:00:01.662894 axsqlalchemy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-06-26 06:59:35.000000 axsqlalchemy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:25.775999 axsqlalchemy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 07:20:25.771999 axsqlalchemy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:25.771999 axsqlalchemy-0.0.3/axsqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/axsqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/axsqlalchemy/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/axsqlalchemy/repository.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/axsqlalchemy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/axsqlalchemy/uow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:20:25.771999 axsqlalchemy-0.0.3/axsqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 07:20:25.000000 axsqlalchemy-0.0.3/axsqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-26 07:20:25.000000 axsqlalchemy-0.0.3/axsqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:20:25.000000 axsqlalchemy-0.0.3/axsqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 07:20:25.000000 axsqlalchemy-0.0.3/axsqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 07:20:25.000000 axsqlalchemy-0.0.3/axsqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 07:20:25.775999 axsqlalchemy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-26 07:19:58.000000 axsqlalchemy-0.0.3/setup.py
```

### Comparing `axsqlalchemy-0.0.1/axsqlalchemy/model.py` & `axsqlalchemy-0.0.3/axsqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.1/axsqlalchemy/repository.py` & `axsqlalchemy-0.0.3/axsqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.1/axsqlalchemy/settings.py` & `axsqlalchemy-0.0.3/axsqlalchemy/settings.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.1/axsqlalchemy/uow.py` & `axsqlalchemy-0.0.3/axsqlalchemy/uow.py`

 * *Files identical despite different names*

