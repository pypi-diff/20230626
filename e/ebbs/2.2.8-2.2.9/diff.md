# Comparing `tmp/ebbs-2.2.8.tar.gz` & `tmp/ebbs-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebbs-2.2.8.tar", last modified: Sun Feb  5 11:23:34 2023, max compression
+gzip compressed data, was "ebbs-2.2.9.tar", last modified: Sun Feb  5 11:50:43 2023, max compression
```

## Comparing `ebbs-2.2.8.tar` & `ebbs-2.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 11:23:34.555265 ebbs-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    17679 2023-02-05 11:23:34.555265 ebbs-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17183 2023-02-05 11:23:19.000000 ebbs-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 11:23:34.551265 ebbs-2.2.8/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 11:23:34.551265 ebbs-2.2.8/pkg/ebbs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-05 11:23:26.000000 ebbs-2.2.8/pkg/ebbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-05 11:23:26.000000 ebbs-2.2.8/pkg/ebbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 11:23:34.555265 ebbs-2.2.8/pkg/ebbs/build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 11:23:26.000000 ebbs-2.2.8/pkg/ebbs/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-05 11:23:08.000000 ebbs-2.2.8/pkg/ebbs/build/build_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-02-05 11:23:26.000000 ebbs-2.2.8/pkg/ebbs/ebbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 11:23:34.551265 ebbs-2.2.8/pkg/ebbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17679 2023-02-05 11:23:34.000000 ebbs-2.2.8/pkg/ebbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-05 11:23:34.000000 ebbs-2.2.8/pkg/ebbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 11:23:34.000000 ebbs-2.2.8/pkg/ebbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-05 11:23:34.000000 ebbs-2.2.8/pkg/ebbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-05 11:23:34.000000 ebbs-2.2.8/pkg/ebbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-05 11:23:34.000000 ebbs-2.2.8/pkg/ebbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-05 11:23:26.000000 ebbs-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-05 11:23:34.555265 ebbs-2.2.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 11:50:43.799928 ebbs-2.2.9/
+-rw-r--r--   0 root         (0) root         (0)    17679 2023-02-05 11:50:43.799928 ebbs-2.2.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    17183 2023-02-05 11:50:22.000000 ebbs-2.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 11:50:43.767928 ebbs-2.2.9/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 11:50:43.779928 ebbs-2.2.9/pkg/ebbs/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-02-05 11:50:27.000000 ebbs-2.2.9/pkg/ebbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-02-05 11:50:27.000000 ebbs-2.2.9/pkg/ebbs/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 11:50:43.799928 ebbs-2.2.9/pkg/ebbs/build/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-05 11:50:27.000000 ebbs-2.2.9/pkg/ebbs/build/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      438 2022-12-27 03:36:04.000000 ebbs-2.2.9/pkg/ebbs/build/build_default.py
+-rw-r--r--   0 root         (0) root         (0)    12863 2023-02-05 11:50:27.000000 ebbs-2.2.9/pkg/ebbs/ebbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 11:50:43.795928 ebbs-2.2.9/pkg/ebbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17679 2023-02-05 11:50:43.000000 ebbs-2.2.9/pkg/ebbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      346 2023-02-05 11:50:43.000000 ebbs-2.2.9/pkg/ebbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-05 11:50:43.000000 ebbs-2.2.9/pkg/ebbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-02-05 11:50:43.000000 ebbs-2.2.9/pkg/ebbs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-02-05 11:50:43.000000 ebbs-2.2.9/pkg/ebbs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-02-05 11:50:43.000000 ebbs-2.2.9/pkg/ebbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-05 11:50:27.000000 ebbs-2.2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      759 2023-02-05 11:50:43.799928 ebbs-2.2.9/setup.cfg
```

### Comparing `ebbs-2.2.8/PKG-INFO` & `ebbs-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebbs
-Version: 2.2.8
+Version: 2.2.9
 Summary: eons Basic Build System
 Home-page: https://github.com/eons-dev/bin_ebbs
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_ebbs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebbs-2.2.8/README.md` & `ebbs-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ebbs-2.2.8/pkg/ebbs/ebbs.py` & `ebbs-2.2.9/pkg/ebbs/ebbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 		# What can this build, "exe", "lib", "img", ... ?
 		this.supportedProjectTypes = []
 
 		this.projectType = None
 		this.projectName = None
 		this.clearBuildPath = False
 
-		this.fetchFrom.remove('globals')
+		try:
+			this.fetchFrom.remove('globals')
+		except:
+			pass
 
 		this.configNameOverrides = {
 			"name": "projectName",
 			"type": "projectType",
 		}
 
 		this.enableRollback = False
```

### Comparing `ebbs-2.2.8/pkg/ebbs.egg-info/PKG-INFO` & `ebbs-2.2.9/pkg/ebbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebbs
-Version: 2.2.8
+Version: 2.2.9
 Summary: eons Basic Build System
 Home-page: https://github.com/eons-dev/bin_ebbs
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_ebbs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebbs-2.2.8/setup.cfg` & `ebbs-2.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ebbs
-version = 2.2.8
+version = 2.2.9
 author = eons
 author_email = support@eons.llc
 description = eons Basic Build System
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_ebbs
@@ -18,16 +18,16 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	eons
 	jsonpickle
+	eons
 
 [options.packages.find]
 where = pkg
 
 [options.entry_points]
 console_scripts = 
 	ebbs = ebbs:ebbs
```

