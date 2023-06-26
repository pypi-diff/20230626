# Comparing `tmp/jolt_docker-0.9.93.tar.gz` & `tmp/jolt_docker-0.9.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jolt_docker-0.9.93.tar", last modified: Mon Apr 24 07:35:16 2023, max compression
+gzip compressed data, was "jolt_docker-0.9.95.tar", last modified: Wed May 10 08:16:59 2023, max compression
```

## Comparing `jolt_docker-0.9.93.tar` & `jolt_docker-0.9.95.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:16.605266 jolt_docker-0.9.93/
--rw-r--r--   0 root         (0) root         (0)     4069 2023-04-24 07:35:16.605266 jolt_docker-0.9.93/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3130 2023-04-21 14:57:08.000000 jolt_docker-0.9.93/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:16.601266 jolt_docker-0.9.93/jolt_docker/
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-21 14:57:08.000000 jolt_docker-0.9.93/jolt_docker/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3308 2023-04-21 14:57:08.000000 jolt_docker-0.9.93/jolt_docker/__main__.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-24 07:23:04.000000 jolt_docker-0.9.93/jolt_docker/version.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-04-21 14:57:08.000000 jolt_docker-0.9.93/jolt_docker/version_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:16.605266 jolt_docker-0.9.93/jolt_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4069 2023-04-24 07:35:16.000000 jolt_docker-0.9.93/jolt_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-24 07:35:16.000000 jolt_docker-0.9.93/jolt_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 07:35:16.000000 jolt_docker-0.9.93/jolt_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-24 07:35:16.000000 jolt_docker-0.9.93/jolt_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 07:35:16.000000 jolt_docker-0.9.93/jolt_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 07:35:16.605266 jolt_docker-0.9.93/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1688 2023-04-21 14:57:08.000000 jolt_docker-0.9.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:16:59.919245 jolt_docker-0.9.95/
+-rw-r--r--   0 root         (0) root         (0)     4069 2023-05-10 08:16:59.919245 jolt_docker-0.9.95/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-04-21 14:57:08.000000 jolt_docker-0.9.95/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:16:59.919245 jolt_docker-0.9.95/jolt_docker/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-21 14:57:08.000000 jolt_docker-0.9.95/jolt_docker/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3308 2023-04-21 14:57:08.000000 jolt_docker-0.9.95/jolt_docker/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-10 08:06:36.000000 jolt_docker-0.9.95/jolt_docker/version.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-04-21 14:57:08.000000 jolt_docker-0.9.95/jolt_docker/version_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:16:59.919245 jolt_docker-0.9.95/jolt_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4069 2023-05-10 08:16:59.000000 jolt_docker-0.9.95/jolt_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-10 08:16:59.000000 jolt_docker-0.9.95/jolt_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:16:59.000000 jolt_docker-0.9.95/jolt_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-10 08:16:59.000000 jolt_docker-0.9.95/jolt_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-10 08:16:59.000000 jolt_docker-0.9.95/jolt_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 08:16:59.919245 jolt_docker-0.9.95/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-21 14:57:08.000000 jolt_docker-0.9.95/setup.py
```

### Comparing `jolt_docker-0.9.93/PKG-INFO` & `jolt_docker-0.9.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolt_docker
-Version: 0.9.93
+Version: 0.9.95
 Summary: A task executor
 Home-page: https://github.com/srand/jolt
 Author: Robert Andersson
 Author-email: srand@github.com
 Keywords: bazel,build,cmake,conan,jolt,make,meson,msbuild,xcode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jolt_docker-0.9.93/README.rst` & `jolt_docker-0.9.95/README.rst`

 * *Files identical despite different names*

### Comparing `jolt_docker-0.9.93/jolt_docker/__main__.py` & `jolt_docker-0.9.95/jolt_docker/__main__.py`

 * *Files identical despite different names*

### Comparing `jolt_docker-0.9.93/jolt_docker/version_utils.py` & `jolt_docker-0.9.95/jolt_docker/version_utils.py`

 * *Files identical despite different names*

### Comparing `jolt_docker-0.9.93/jolt_docker.egg-info/PKG-INFO` & `jolt_docker-0.9.95/jolt_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolt-docker
-Version: 0.9.93
+Version: 0.9.95
 Summary: A task executor
 Home-page: https://github.com/srand/jolt
 Author: Robert Andersson
 Author-email: srand@github.com
 Keywords: bazel,build,cmake,conan,jolt,make,meson,msbuild,xcode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jolt_docker-0.9.93/setup.py` & `jolt_docker-0.9.95/setup.py`

 * *Files identical despite different names*

