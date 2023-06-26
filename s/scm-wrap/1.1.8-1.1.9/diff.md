# Comparing `tmp/scm-wrap-1.1.8.tar.gz` & `tmp/scm-wrap-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scm-wrap-1.1.8.tar", last modified: Fri Feb  3 16:11:34 2023, max compression
+gzip compressed data, was "scm-wrap-1.1.9.tar", last modified: Fri Feb  3 17:50:30 2023, max compression
```

## Comparing `scm-wrap-1.1.8.tar` & `scm-wrap-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-02-03 16:11:34.724968 scm-wrap-1.1.8/
--rw-r--r--   0 mello     (1000) mello     (1000)      439 2023-02-03 16:11:34.724968 scm-wrap-1.1.8/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      415 2023-01-12 09:45:07.000000 scm-wrap-1.1.8/README.md
--rw-r--r--   0 mello     (1000) mello     (1000)      661 2023-01-31 10:53:19.000000 scm-wrap-1.1.8/pyproject.toml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-02-03 16:11:34.721635 scm-wrap-1.1.8/scm_wrap.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      439 2023-02-03 16:11:34.000000 scm-wrap-1.1.8/scm_wrap.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      254 2023-02-03 16:11:34.000000 scm-wrap-1.1.8/scm_wrap.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-02-03 16:11:34.000000 scm-wrap-1.1.8/scm_wrap.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-02-03 16:11:34.000000 scm-wrap-1.1.8/scm_wrap.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-02-03 16:11:34.724968 scm-wrap-1.1.8/scmwrap/
--rw-r--r--   0 mello     (1000) mello     (1000)      100 2023-01-12 09:45:07.000000 scm-wrap-1.1.8/scmwrap/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)    13228 2023-01-31 10:53:14.000000 scm-wrap-1.1.8/scmwrap/git.py
--rw-r--r--   0 mello     (1000) mello     (1000)        0 2023-01-12 09:45:07.000000 scm-wrap-1.1.8/scmwrap/py.typed
--rw-r--r--   0 mello     (1000) mello     (1000)     6855 2023-01-31 10:53:14.000000 scm-wrap-1.1.8/scmwrap/repo.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1843 2023-01-17 09:55:01.000000 scm-wrap-1.1.8/scmwrap/scmwrap.py
--rw-r--r--   0 mello     (1000) mello     (1000)     9955 2023-01-31 10:53:14.000000 scm-wrap-1.1.8/scmwrap/svn.py
--rw-r--r--   0 mello     (1000) mello     (1000)       38 2023-02-03 16:11:34.724968 scm-wrap-1.1.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 17:50:30.372533 scm-wrap-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-02-03 17:50:30.372533 scm-wrap-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-01-16 10:33:38.000000 scm-wrap-1.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-02-03 16:50:26.000000 scm-wrap-1.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-01-16 10:33:38.000000 scm-wrap-1.1.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 17:50:30.368533 scm-wrap-1.1.9/scm_wrap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-02-03 17:50:30.000000 scm-wrap-1.1.9/scm_wrap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      302 2023-02-03 17:50:30.000000 scm-wrap-1.1.9/scm_wrap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 17:50:30.000000 scm-wrap-1.1.9/scm_wrap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-02-03 17:50:30.000000 scm-wrap-1.1.9/scm_wrap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-02-03 17:50:30.000000 scm-wrap-1.1.9/scm_wrap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 17:50:30.372533 scm-wrap-1.1.9/scmwrap/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-01-16 10:33:38.000000 scm-wrap-1.1.9/scmwrap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13228 2023-01-29 22:32:22.000000 scm-wrap-1.1.9/scmwrap/git.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-03 17:49:37.000000 scm-wrap-1.1.9/scmwrap/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     6855 2023-01-29 22:32:22.000000 scm-wrap-1.1.9/scmwrap/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-01-17 09:47:37.000000 scm-wrap-1.1.9/scmwrap/scmwrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2023-01-29 22:32:22.000000 scm-wrap-1.1.9/scmwrap/svn.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-03 17:50:30.372533 scm-wrap-1.1.9/setup.cfg
```

### Comparing `scm-wrap-1.1.8/pyproject.toml` & `scm-wrap-1.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scm-wrap"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
     { name="Marco Bascetta", email="m.bascetta@zohomail.eu" },
     { name="Matteo Martelli", email="matteomartelli3@gmail.com" },
     { name="Marco Melletti", email="melletti.marco@gmail.com" },
 ]
 description = "Source Code Management module wrapper. This module aims to wrap access to Git, Subversion and other SCMs repositories"
 requires-python = ">=3.7"
+dynamic = ["dependencies"]
+
 classifiers = [
    "Programming Language :: Python :: 3",
    "Operating System :: OS Independent",
 ]
 
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+
 [tool.setuptools.package-data]
 "scmwrap" = ["py.typed"]
```

### Comparing `scm-wrap-1.1.8/scmwrap/git.py` & `scm-wrap-1.1.9/scmwrap/git.py`

 * *Files identical despite different names*

### Comparing `scm-wrap-1.1.8/scmwrap/repo.py` & `scm-wrap-1.1.9/scmwrap/repo.py`

 * *Files identical despite different names*

### Comparing `scm-wrap-1.1.8/scmwrap/scmwrap.py` & `scm-wrap-1.1.9/scmwrap/scmwrap.py`

 * *Files identical despite different names*

### Comparing `scm-wrap-1.1.8/scmwrap/svn.py` & `scm-wrap-1.1.9/scmwrap/svn.py`

 * *Files identical despite different names*

