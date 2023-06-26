# Comparing `tmp/check-python-versions-0.9.1.tar.gz` & `tmp/check-python-versions-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/check-python-versions-0.9.1.tar", last modified: Fri Nov 30 16:47:46 2018, max compression
+gzip compressed data, was "dist/check-python-versions-0.9.2.tar", last modified: Mon Dec  3 20:51:16 2018, max compression
```

## Comparing `check-python-versions-0.9.1.tar` & `check-python-versions-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/
--rw-r--r--   0 mg        (1000) mg        (1000)     9870 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)    35149 2018-11-16 14:31:10.000000 check-python-versions-0.9.1/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)       29 2018-11-16 16:18:29.000000 check-python-versions-0.9.1/.gitignore
--rwxr-xr-x   0 mg        (1000) mg        (1000)    13077 2018-11-30 16:47:33.000000 check-python-versions-0.9.1/check-python-versions
--rw-r--r--   0 mg        (1000) mg        (1000)      350 2018-11-30 16:47:33.000000 check-python-versions-0.9.1/CHANGES.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      168 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)      122 2018-11-16 15:58:25.000000 check-python-versions-0.9.1/Makefile
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/check_python_versions.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)      382 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/check_python_versions.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     9870 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/check_python_versions.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2018-11-16 16:00:12.000000 check-python-versions-0.9.1/check_python_versions.egg-info/not-zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/check_python_versions.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        7 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/check_python_versions.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2018-11-30 16:47:46.000000 check-python-versions-0.9.1/check_python_versions.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     4067 2018-11-16 15:57:33.000000 check-python-versions-0.9.1/release.mk
--rwxr-xr-x   0 mg        (1000) mg        (1000)     1441 2018-11-16 16:00:04.000000 check-python-versions-0.9.1/setup.py
--rw-r--r--   0 mg        (1000) mg        (1000)       79 2018-11-16 16:18:41.000000 check-python-versions-0.9.1/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)     7241 2018-11-30 16:39:20.000000 check-python-versions-0.9.1/README.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/
+-rw-r--r--   0 mg        (1000) mg        (1000)     9870 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)    35149 2018-11-16 14:31:10.000000 check-python-versions-0.9.2/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)       29 2018-11-16 16:18:29.000000 check-python-versions-0.9.2/.gitignore
+-rwxr-xr-x   0 mg        (1000) mg        (1000)    13095 2018-12-03 20:51:01.000000 check-python-versions-0.9.2/check-python-versions
+-rw-r--r--   0 mg        (1000) mg        (1000)      433 2018-12-03 20:51:01.000000 check-python-versions-0.9.2/CHANGES.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      168 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/setup.cfg
+-rw-r--r--   0 mg        (1000) mg        (1000)      122 2018-11-16 15:58:25.000000 check-python-versions-0.9.2/Makefile
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/check_python_versions.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)      382 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/check_python_versions.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     9870 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/check_python_versions.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2018-11-16 16:00:12.000000 check-python-versions-0.9.2/check_python_versions.egg-info/not-zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/check_python_versions.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        7 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/check_python_versions.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2018-12-03 20:51:16.000000 check-python-versions-0.9.2/check_python_versions.egg-info/top_level.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     4067 2018-11-16 15:57:33.000000 check-python-versions-0.9.2/release.mk
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     1441 2018-11-16 16:00:04.000000 check-python-versions-0.9.2/setup.py
+-rw-r--r--   0 mg        (1000) mg        (1000)       79 2018-11-16 16:18:41.000000 check-python-versions-0.9.2/MANIFEST.in
+-rw-r--r--   0 mg        (1000) mg        (1000)     7241 2018-11-30 16:39:20.000000 check-python-versions-0.9.2/README.rst
```

### Comparing `check-python-versions-0.9.1/PKG-INFO` & `check-python-versions-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: check-python-versions
-Version: 0.9.1
+Version: 0.9.2
 Summary: Compare supported Python versions in setup.py vs tox.ini et al.
 Home-page: https://github.com/mgedmin/check-python-versions
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL
 Description: check-python-versions
         =====================
```

### Comparing `check-python-versions-0.9.1/LICENSE` & `check-python-versions-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `check-python-versions-0.9.1/check-python-versions` & `check-python-versions-0.9.2/check-python-versions`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     import yaml
 except ImportError:
     yaml = None
     print("pyaml is needed for .travis.yml support (apt install python3-yaml)")
 
 
 __author__ = 'Marius Gedminas <marius@gedmin.as>'
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 
 log = logging.getLogger('check-python-versions')
 
 
 TOX_INI = 'tox.ini'
 TRAVIS_YML = '.travis.yml'
@@ -71,19 +71,19 @@
 def get_versions_from_classifiers(classifiers):
     # Based on
     # https://github.com/mgedmin/project-summary/blob/master/summary.py#L221-L234
     prefix = 'Programming Language :: Python :: '
     impl_prefix = 'Programming Language :: Python :: Implementation :: '
     cpython = impl_prefix + 'CPython'
     versions = {
-        s[len(prefix):].replace(' :: Only', '')
+        s[len(prefix):].replace(' :: Only', '').rstrip()
         for s in classifiers
         if s.startswith(prefix) and s[len(prefix):len(prefix) + 1].isdigit()
     } | {
-        s[len(impl_prefix):]
+        s[len(impl_prefix):].rstrip()
         for s in classifiers
         if s.startswith(impl_prefix) and s != cpython
     }
     for major in '2', '3':
         if major in versions and any(
                 v.startswith(f'{major}.') for v in versions):
             versions.remove(major)
```

### Comparing `check-python-versions-0.9.1/check_python_versions.egg-info/PKG-INFO` & `check-python-versions-0.9.2/check_python_versions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: check-python-versions
-Version: 0.9.1
+Version: 0.9.2
 Summary: Compare supported Python versions in setup.py vs tox.ini et al.
 Home-page: https://github.com/mgedmin/check-python-versions
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL
 Description: check-python-versions
         =====================
```

### Comparing `check-python-versions-0.9.1/release.mk` & `check-python-versions-0.9.2/release.mk`

 * *Files identical despite different names*

### Comparing `check-python-versions-0.9.1/setup.py` & `check-python-versions-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `check-python-versions-0.9.1/README.rst` & `check-python-versions-0.9.2/README.rst`

 * *Files identical despite different names*

