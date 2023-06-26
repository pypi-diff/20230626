# Comparing `tmp/roman_datamodels-0.8.0.tar.gz` & `tmp/roman_datamodels-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpds_kkz1r/tmpds2gto81/roman_datamodels-0.8.0.tar", last modified: Mon Nov 22 20:04:57 2021, max compression
+gzip compressed data, was "roman_datamodels-0.9.0.tar", last modified: Fri Feb  4 22:08:21 2022, max compression
```

## Comparing `roman_datamodels-0.8.0.tar` & `roman_datamodels-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/
--rw-r--r--   0 root         (0) root         (0)      192 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      752 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/tox.ini
--rw-r--r--   0 root         (0) root         (0)     2098 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1463 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2535 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/CHANGES.rst
--rw-r--r--   0 root         (0) root         (0)     1047 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1420 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      846 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 root         (0) root         (0)     2592 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     1964 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1035 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/CONTRIBUTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1677 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/tests/test_stnode.py
--rw-r--r--   0 root         (0) root         (0)      213 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1476 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/tests/test_factories.py
--rw-r--r--   0 root         (0) root         (0)    14156 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     2819 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/tests/test_open.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      954 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/scripts/set_release_date
--rwxr-xr-x   0 root         (0) root         (0)      986 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/scripts/insert_next_release
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      349 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      218 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)      179 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1047 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1289 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       82 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels.egg-info/entry_points.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels/
--rw-r--r--   0 root         (0) root         (0)     2384 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/validate.py
--rw-r--r--   0 root         (0) root         (0)     8492 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/mktest.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13935 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/datamodels.py
--rw-r--r--   0 root         (0) root         (0)     6631 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/stnode_test.py
--rw-r--r--   0 root         (0) root         (0)    12898 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/stnode.py
--rw-r--r--   0 root         (0) root         (0)      380 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/extensions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels/testing/
--rw-r--r--   0 root         (0) root         (0)      217 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17798 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/testing/utils.py
--rw-r--r--   0 root         (0) root         (0)     1380 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/testing/assertions.py
--rw-r--r--   0 root         (0) root         (0)    29835 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/testing/factories.py
--rw-r--r--   0 root         (0) root         (0)     2986 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/stuserdict.py
--rw-r--r--   0 root         (0) root         (0)      313 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/integration.py
--rw-r--r--   0 root         (0) root         (0)      178 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/table_definitions.py
--rw-r--r--   0 root         (0) root         (0)     1248 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/filetype.py
--rw-r--r--   0 root         (0) root         (0)      142 2021-11-22 20:04:57.000000 roman_datamodels-0.8.0/src/roman_datamodels/_version.py
--rw-r--r--   0 root         (0) root         (0)    16232 2021-11-22 20:04:22.000000 roman_datamodels-0.8.0/src/roman_datamodels/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.969992 roman_datamodels-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.961991 roman_datamodels-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.965991 roman_datamodels-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3101 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-02-04 22:08:21.969992 roman_datamodels-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.965991 roman_datamodels-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      986 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/scripts/insert_next_release
+-rwxr-xr-x   0 runner    (1001) docker     (121)      954 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/scripts/set_release_date
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-02-04 22:08:21.969992 roman_datamodels-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.961991 roman_datamodels-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.965991 roman_datamodels-0.9.0/src/roman_datamodels/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13985 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/datamodels.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8492 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/mktest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12805 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/stnode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6631 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/stnode_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/stuserdict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.969992 roman_datamodels-0.9.0/src/roman_datamodels/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/testing/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30318 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/testing/factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25433 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16234 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/src/roman_datamodels/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.969992 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 22:08:21.000000 roman_datamodels-0.9.0/src/roman_datamodels.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:08:21.969992 roman_datamodels-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/tests/test_factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15577 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/tests/test_stnode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-02-04 22:08:10.000000 roman_datamodels-0.9.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `roman_datamodels-0.8.0/tox.ini` & `roman_datamodels-0.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist= py38,style,bandit
+envlist= py38,py310,style,bandit
 
 [testenv]
 extras= test
 # astropy will complain if the home directory is missing
 passenv= HOME
 commands=
     pytest
```

### Comparing `roman_datamodels-0.8.0/.gitignore` & `roman_datamodels-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/LICENSE` & `roman_datamodels-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/CHANGES.rst` & `roman_datamodels-0.9.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+0.9.0 (2022-02-04)
+==================
+
+- Updated rampfit and flat maker utilities to support the same functionality as the other model maker functions. Streamlined and commented all maker utility functions. Added tests to complete coverage of roman_datamodels/testing/utils.py. Cleaned out some deprecated code. [#59]
+
+- Updated stnode tests to include all cal steps. [#60]
+
+- Fix bug with asdf 2.9.x due to change in private variable name. [#63]
+
 0.8.0 (2021-11-22)
 ==================
 
 - Add support for the cal_logs array, which will be used to store calibration
   log messages. [#53]
 
 0.7.0 (2021-11-10)
 ==================
 
+- Modified DNode and LNode classes to provide asdf info method introspection
+  into the contents of the class. [#61]
+
 - Modified open function to handle accepting model instances that are checked
   against a target datamodel class, whether supplied directly as a model instance,
   or obtained by the referenced ASDF file. [#52]
 
 - Created maker utility and tests for ramp_fit_output files. [#50]
 
 0.6.0 (2021-10-26)
```

### Comparing `roman_datamodels-0.8.0/PKG-INFO` & `roman_datamodels-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roman_datamodels
-Version: 0.8.0
+Version: 0.9.0
 Summary: Roman Datamodels
 Home-page: https://github.com/spacetelescope/roman_datamodels
 Author: STScI
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/spacetelescope/roman_datamodels/issues
 Project-URL: Source Code, https://github.com/spacetelescope/roman_datamodels
 Platform: UNKNOWN
```

### Comparing `roman_datamodels-0.8.0/setup.cfg` & `roman_datamodels-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [options]
 zip_safe = True
 python_requires = >=3.6
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	jsonschema>=3.0.2
-	asdf>=2.8.0
+	asdf>=2.9.1
 	psutil>=5.7.2
 	numpy>=1.16
 	astropy>=4.0
 	romanad>=0.8.0
 package_dir = 
 	=src
 packages = find:
```

### Comparing `roman_datamodels-0.8.0/.github/workflows/ci.yml` & `roman_datamodels-0.9.0/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,18 @@
   tox:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
         include:
+          - name: Python 3.10
+            runs-on: ubuntu-latest
+            python-version: "3.10"
+            toxenv: py310
           - name: Python 3.9
             runs-on: ubuntu-latest
             python-version: 3.9
             toxenv: py39
 
           - name: Python 3.8
             runs-on: ubuntu-latest
```

### Comparing `roman_datamodels-0.8.0/.github/workflows/release.yml` & `roman_datamodels-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/CONTRIBUTING.md` & `roman_datamodels-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/tests/test_stnode.py` & `roman_datamodels-0.9.0/tests/test_stnode.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,7 +46,19 @@
     node = create_node(node_class)
     with asdf.AsdfFile() as af:
         af["node"] = node
         af.write_to(file_path)
 
     with asdf.open(file_path) as af:
         assert_node_equal(af["node"], node)
+
+
+def test_info(capsys):
+    node = stnode.WfiMode({"optical_element": "GRISM",
+                           "detector": "WFI18",
+                           "name": "WFI"})
+    tree = dict(wfimode=node)
+    af = asdf.AsdfFile(tree)
+    af.info()
+    captured = capsys.readouterr()
+    assert "optical_element" in captured.out
+    assert "GRISM" in captured.out
```

### Comparing `roman_datamodels-0.8.0/tests/test_factories.py` & `roman_datamodels-0.9.0/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/tests/test_models.py` & `roman_datamodels-0.9.0/tests/test_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,48 +2,44 @@
 
 from jsonschema import ValidationError
 import asdf
 import numpy as np
 
 from roman_datamodels import datamodels
 from roman_datamodels import stnode
-# from roman_datamodels import table_definitions
 from roman_datamodels.extensions import DATAMODEL_EXTENSIONS
 
 from roman_datamodels.testing import utils
 
 
 EXPECTED_COMMON_REFERENCE = \
     {'$ref': 'ref_common-1.0.0'}
 
-# Helper class to iterate over model subclasses
-
 
+# Helper class to iterate over model subclasses
 def iter_subclasses(model_class, include_base_model=True):
     if include_base_model:
         yield model_class
     for sub_class in model_class.__subclasses__():
         yield from iter_subclasses(sub_class)
 
 
 def test_model_schemas():
     dmodels = datamodels.model_registry.keys()
     for model in dmodels:
         schema_uri = next(t for t in DATAMODEL_EXTENSIONS[0].tags
-                          if t._tag_uri == model._tag)._schema_uri
+                          if t._tag_uri == model._tag).schema_uris[0]
         asdf.schema.load_schema(schema_uri)
 
 # Testing core schema
-
-
 def test_core_schema(tmp_path):
     # Set temporary asdf file
     file_path = tmp_path / "test.asdf"
 
-    wfi_image = utils.mk_level2_image(arrays=(10, 10))
+    wfi_image = utils.mk_level2_image(shape=(10, 10))
     with asdf.AsdfFile() as af:
         af.tree = {'roman': wfi_image}
         with pytest.raises(ValidationError):
             af.tree['roman'].meta.telescope = 'NOTROMAN'
         af.tree['roman'].meta['telescope'] = 'NOTROMAN'
         with pytest.raises(ValidationError):
             af.write_to(file_path)
@@ -61,19 +57,44 @@
         with datamodels.open(file_path) as model:
             pass
     asdf.get_config().validate_on_read = False
     with datamodels.open(file_path) as model:
         assert model.meta.telescope == 'XOMAN'
     asdf.get_config().validate_on_read = True
 
+
 # RampFitOutput tests
+def test_make_ramp():
+    ramp = utils.mk_ramp(shape=(2, 20, 20))
+
+    assert ramp.meta.exposure.type == 'WFI_IMAGE'
+    assert ramp.data.dtype == np.float32
+    assert ramp.pixeldq.dtype == np.uint32
+    assert ramp.pixeldq.shape == (20, 20)
+    assert ramp.groupdq.dtype == np.uint8
+    assert ramp.err.dtype == np.float32
+    assert ramp.err.shape == (20, 20)
 
+    # Test validation
+    ramp = datamodels.RampModel(ramp)
+    assert ramp.validate() is None
+
+
+def test_opening_ramp_ref(tmp_path):
+    # First make test reference file
+    file_path = tmp_path / 'testramp.asdf'
+    utils.mk_ramp(filepath=file_path)
+    ramp = datamodels.open(file_path)
+    assert ramp.meta.instrument.optical_element == 'F062'
+    assert isinstance(ramp, datamodels.RampModel)
 
+
+# RampFitOutput tests
 def test_make_rampfitoutput():
-    rampfitoutput = utils.mk_rampfitoutput(arrays=(2, 20, 20))
+    rampfitoutput = utils.mk_rampfitoutput(shape=(2, 20, 20))
 
     assert rampfitoutput.meta.exposure.type == 'WFI_IMAGE'
     assert rampfitoutput.slope.dtype == np.float32
     assert rampfitoutput.sigslope.dtype == np.float32
     assert rampfitoutput.yint.dtype == np.float32
     assert rampfitoutput.sigyint.dtype == np.float32
     assert rampfitoutput.pedestal.dtype == np.float32
@@ -94,42 +115,54 @@
     file_path = tmp_path / 'testrampfitoutput.asdf'
     utils.mk_rampfitoutput(filepath=file_path)
     rampfitoutput = datamodels.open(file_path)
     assert rampfitoutput.meta.instrument.optical_element == 'F062'
     assert isinstance(rampfitoutput, datamodels.RampFitOutputModel)
 
 
+
 # Testing all reference file schemas
 def test_reference_file_model_base(tmp_path):
     # Set temporary asdf file
 
     # Get all reference file classes
-    tags = [t for t in DATAMODEL_EXTENSIONS[0].tags if "/reference_files/" in t._tag_uri]
+    tags = [t for t in DATAMODEL_EXTENSIONS[0].tags if "/reference_files/" in t.tag_uri]
     for tag in tags:
-        schema = asdf.schema.load_schema(tag._schema_uri)
+        schema = asdf.schema.load_schema(tag.schema_uris[0])
         # Check that schema references common reference schema
         allofs = schema['properties']['meta']['allOf']
         found_common = False
         for item in allofs:
             if item == EXPECTED_COMMON_REFERENCE:
                 found_common = True
         if not found_common:
             raise ValueError("Reference schema does not include ref_common")
 
 
+# Flat tests
+def test_make_flat():
+    flat = utils.mk_flat(shape=(20, 20))
+    assert flat.meta.reftype == 'FLAT'
+    assert flat.data.dtype == np.float32
+    assert flat.dq.dtype == np.uint32
+    assert flat.dq.shape == (20, 20)
+    assert flat.err.dtype == np.float32
+
+    # Test validation
+    flat_model = datamodels.FlatRefModel(flat)
+    assert flat_model.validate() is None
+
 def test_opening_flat_ref(tmp_path):
     # First make test reference file
     file_path = tmp_path / 'testflat.asdf'
-    utils.mk_flat_file(file_path)
+    utils.mk_flat(filepath=file_path)
     flat = datamodels.open(file_path)
     assert flat.meta.instrument.optical_element == 'F158'
     assert isinstance(flat, datamodels.FlatRefModel)
 
-
-# FlatModel tests
 def test_flat_model(tmp_path):
     # Set temporary asdf file
     file_path = tmp_path / "test.asdf"
 
     meta = {}
     utils.add_ref_common(meta)
     meta['reftype'] = "FLAT"
@@ -150,31 +183,14 @@
         with datamodels.open(file_path) as model:
             with pytest.warns(None):
                 model.validate()
 
             # Confirm that asdf file is opened as flat file model
             assert isinstance(model, datamodels.FlatRefModel)
 
-# not sure what the following is supposed to ensure PG
-
-# def test_meta_date_management(tmp_path):
-#     model = datamodels.RomanDataModel({
-#         "meta": {
-#             "date": Time("2000-01-01T00:00:00.000"),
-#             "instrument": {"name": "WFI", "detector": "WFI01", "optical_element": "F062"},
-#             "telescope": "ROMAN",
-#         }
-#     })
-#     assert model.meta.date == Time("2000-01-01T00:00:00.000")
-#     model.save(str(tmp_path/"test.asdf"))
-#     assert abs((Time.now() - model.meta.date).value) < 1.0
-
-#     model = datamodels.RomanDataModel()
-#     assert abs((Time.now() - model.meta.date).value) < 1.0
-
 
 # Dark Current tests
 def test_make_dark():
     dark = utils.mk_dark(shape=(3, 20, 20))
     assert dark.meta.reftype == 'DARK'
     assert dark.data.dtype == np.float32
     assert dark.dq.dtype == np.uint32
@@ -190,17 +206,16 @@
     # First make test reference file
     file_path = tmp_path / 'testdark.asdf'
     utils.mk_dark(filepath=file_path)
     dark = datamodels.open(file_path)
     assert dark.meta.instrument.optical_element == 'F158'
     assert isinstance(dark, datamodels.DarkRefModel)
 
-# Gain tests
-
 
+# Gain tests
 def test_make_gain():
     gain = utils.mk_gain(shape=(20, 20))
     assert gain.meta.reftype == 'GAIN'
     assert gain.data.dtype == np.float32
 
     # Test validation
     gain_model = datamodels.GainRefModel(gain)
@@ -252,17 +267,16 @@
     # First make test reference file
     file_path = tmp_path / 'testmask.asdf'
     utils.mk_mask(filepath=file_path)
     mask = datamodels.open(file_path)
     assert mask.meta.instrument.optical_element == 'F158'
     assert isinstance(mask, datamodels.MaskRefModel)
 
-# Pixel Area tests
-
 
+# Pixel Area tests
 def test_make_pixelarea():
     pixearea = utils.mk_pixelarea(shape=(20, 20))
     assert pixearea.meta.reftype == 'AREA'
     assert type(pixearea.meta.photometry.pixelarea_steradians) == float
     assert type(pixearea.meta.photometry.pixelarea_arcsecsq) == float
     assert pixearea.data.dtype == np.float32
 
@@ -275,17 +289,16 @@
     # First make test reference file
     file_path = tmp_path / 'testpixelarea.asdf'
     utils.mk_pixelarea(filepath=file_path)
     pixelarea = datamodels.open(file_path)
     assert pixelarea.meta.instrument.optical_element == 'F158'
     assert isinstance(pixelarea, datamodels.PixelareaRefModel)
 
-# Read Noise tests
-
 
+# Read Noise tests
 def test_make_readnoise():
     readnoise = utils.mk_readnoise(shape=(20, 20))
     assert readnoise.meta.reftype == 'READNOISE'
     assert readnoise.data.dtype == np.float32
 
     # Test validation
     readnoise_model = datamodels.ReadnoiseRefModel(readnoise)
@@ -335,17 +348,16 @@
     # First make test reference file
     file_path = tmp_path / 'testsaturation.asdf'
     utils.mk_saturation(filepath=file_path)
     saturation = datamodels.open(file_path)
     assert saturation.meta.instrument.optical_element == 'F158'
     assert isinstance(saturation, datamodels.SaturationRefModel)
 
-# Super Bias tests
-
 
+# Super Bias tests
 def test_make_superbias():
     superbias = utils.mk_superbias(shape=(20, 20))
     assert superbias.meta.reftype == 'BIAS'
     assert superbias.data.dtype == np.float32
     assert superbias.err.dtype == np.float32
     assert superbias.dq.dtype == np.uint32
     assert superbias.dq.shape == (20, 20)
@@ -359,17 +371,16 @@
     # First make test reference file
     file_path = tmp_path / 'testsuperbias.asdf'
     utils.mk_superbias(filepath=file_path)
     superbias = datamodels.open(file_path)
     assert superbias.meta.instrument.optical_element == 'F158'
     assert isinstance(superbias, datamodels.SuperbiasRefModel)
 
-# WHI Photom tests
-
 
+# WFI Photom tests
 def test_make_wfi_img_photom():
     wfi_img_photom = utils.mk_wfi_img_photom()
 
     assert wfi_img_photom.meta.reftype == 'PHOTOM'
     assert type(wfi_img_photom.phot_table.W146.photmjsr) == float
     assert type(wfi_img_photom.phot_table.F184.photmjsr) == float
     assert type(wfi_img_photom.phot_table.W146.uncertainty) == float
@@ -386,33 +397,66 @@
     utils.mk_wfi_img_photom(filepath=file_path)
     wfi_img_photom = datamodels.open(file_path)
 
     assert wfi_img_photom.meta.instrument.optical_element == 'F158'
     assert isinstance(wfi_img_photom, datamodels.WfiImgPhotomRefModel)
 
 
-def test_open_with_model_class(tmp_path):
+# WFI Level 1 Science Raw tests
+def test_level1_science_raw():
+    wfi_science_raw = utils.mk_level1_science_raw()
+
+    assert wfi_science_raw.data.dtype == np.uint16
+
+    # Test validation
+    wfi_science_raw_model = datamodels.ScienceRawModel(wfi_science_raw)
+    assert wfi_science_raw_model.validate() is None
+
+
+def test_opening_level1_science_raw(tmp_path):
     # First make test reference file
-    file_path = tmp_path / 'testreadnoise.asdf'
-    utils.mk_readnoise(filepath=file_path)
-    rnmod = datamodels.ReadnoiseRefModel(file_path)
-    assert rnmod.meta.reftype == "READNOISE"
-    assert rnmod.data.shape == (4096, 4224)
-    with pytest.raises(ValueError):
-        datamodels.RampModel(file_path)
+    file_path = tmp_path / 'testwfi_science_raw.asdf'
+    utils.mk_level1_science_raw(filepath=file_path)
+    wfi_science_raw = datamodels.open(file_path)
 
+    assert wfi_science_raw.meta.instrument.optical_element == 'F062'
+    assert isinstance(wfi_science_raw, datamodels.ScienceRawModel)
 
-def test_open_with_target(tmp_path):
-    file_path = tmp_path / 'testreadnoise.asdf'
-    utils.mk_readnoise(filepath=file_path)
-    rnmod = datamodels.ReadnoiseRefModel(file_path)
-    rnmod2 = datamodels.open(rnmod, target=datamodels.ReadnoiseRefModel)
-    assert rnmod is rnmod2
-    rnmod3 = datamodels.open(rnmod)
-    assert rnmod3 is not rnmod
-    with pytest.raises(ValueError):
-        datamodels.open(rnmod, target=datamodels.WfiImgPhotomRefModel)
-    with pytest.raises(ValueError):
-        datamodels.open(
-            file_path, target=datamodels.WfiImgPhotomRefModel)
-    with pytest.raises((ValueError, TypeError)):
-        datamodels.open(file_path, target='bullseye')
+
+# WFI Level 2 Image tests
+def test_level2_image():
+    wfi_image = utils.mk_level2_image()
+
+    assert wfi_image.data.dtype == np.float32
+    assert wfi_image.dq.dtype == np.uint32
+    assert wfi_image.err.dtype == np.float32
+    assert wfi_image.var_poisson.dtype == np.float32
+    assert wfi_image.var_rnoise.dtype == np.float32
+    assert wfi_image.var_flat.dtype == np.float32
+    assert wfi_image.area.dtype == np.float32
+    assert type(wfi_image.cal_logs[0]) == str
+
+    # Test validation
+    wfi_image_model = datamodels.ImageModel(wfi_image)
+    assert wfi_image_model.validate() is None
+
+
+def test_opening_level2_image(tmp_path):
+    # First make test reference file
+    file_path = tmp_path / 'testwfi_image.asdf'
+    utils.mk_level2_image(filepath=file_path)
+    wfi_image = datamodels.open(file_path)
+
+    assert wfi_image.meta.instrument.optical_element == 'F062'
+    assert isinstance(wfi_image, datamodels.ImageModel)
+
+def test_datamodel_info_search(capsys):
+    wfi_science_raw = utils.mk_level1_science_raw()
+    af = asdf.AsdfFile()
+    af.tree = {'roman': wfi_science_raw}
+    dm = datamodels.open(af)
+    dm.info(max_rows=200)
+    captured = capsys.readouterr()
+    assert "optical_element" in captured.out
+    result = dm.search('optical_element')
+    assert 'F062' in repr(result)
+    assert result.node == 'F062'
```

### Comparing `roman_datamodels-0.8.0/tests/test_open.py` & `roman_datamodels-0.9.0/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/scripts/set_release_date` & `roman_datamodels-0.9.0/scripts/set_release_date`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/scripts/insert_next_release` & `roman_datamodels-0.9.0/scripts/insert_next_release`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels.egg-info/PKG-INFO` & `roman_datamodels-0.9.0/src/roman_datamodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roman-datamodels
-Version: 0.8.0
+Version: 0.9.0
 Summary: Roman Datamodels
 Home-page: https://github.com/spacetelescope/roman_datamodels
 Author: STScI
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/spacetelescope/roman_datamodels/issues
 Project-URL: Source Code, https://github.com/spacetelescope/roman_datamodels
 Platform: UNKNOWN
```

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels.egg-info/SOURCES.txt` & `roman_datamodels-0.9.0/src/roman_datamodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/validate.py` & `roman_datamodels-0.9.0/src/roman_datamodels/validate.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/mktest.py` & `roman_datamodels-0.9.0/src/roman_datamodels/mktest.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/datamodels.py` & `roman_datamodels-0.9.0/src/roman_datamodels/datamodels.py`

 * *Files 3% similar despite different names*

```diff
@@ -272,19 +272,19 @@
     def validate(self):
         """
         Re-validate the model instance against the tags
         """
         validate.value_change(self._instance, pass_invalid_values=False,
                               strict_validation=True)
 
-    # def __getitem__(self, key):
-    #   assert isinstance(key, str)
+    def info(self, *args, **kwargs):
+        return self._asdf.info(*args, **kwargs)
 
-    # def __setitem__(self, key, value):
-    #   pass
+    def search(self, *args, **kwargs):
+        return self._asdf.search(*args, **kwargs)
 
 
 class ImageModel(DataModel):
     pass
 
 
 class ScienceRawModel(DataModel):
```

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/stnode_test.py` & `roman_datamodels-0.9.0/src/roman_datamodels/stnode_test.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/stnode.py` & `roman_datamodels-0.9.0/src/roman_datamodels/stnode.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         'http://stsci.edu/schemas/asdf-schema/0.1.0/asdf-schema'}
     temp_schema.update(schema)
     validator = asdfschema.get_validator(temp_schema,
                                          validator_context,
                                          validator_callbacks,
                                          validator_resolver)
 
-    #value = yamlutil.custom_tree_to_tagged_tree(value, validator_context)
     validator.validate(value, _schema=temp_schema)
     validator_context.close()
 
 
 def _validate(attr, instance, schema, ctx):
     tagged_tree = yamlutil.custom_tree_to_tagged_tree(instance, ctx)
     return _value_change(attr, tagged_tree, schema, False, strict_validation, ctx)
@@ -219,19 +218,18 @@
         the parent class, recursing if necessary until one is found.
         """
         if self._x_schema is None:
             parent_schema = self._parent._schema()
             # Extract the subschema corresponding to this node.
             subschema = _get_schema_for_property(parent_schema, self._name)
             self._x_schema = subschema
-    # def __getindex__(self, key):
-    #     return self.data[key]
 
-    # def __setindex__(self, key, value):
-    #     self.data[key] = value
+    def __asdf_traverse__(self):
+        return dict(self)
+
 
 class LNode(UserList):
 
     _tag = None
 
     def __init__(self, node=None):
         if node is None:
@@ -248,14 +246,17 @@
         if isinstance(value, dict):
             return DNode(value)
         elif isinstance(value, list):
             return LNode(value)
         else:
             return value
 
+    def __asdf_traverse__(self):
+        return list(self)
+
 
 _OBJECT_NODE_CLASSES_BY_TAG = {}
 
 
 class TaggedObjectNodeMeta(ABCMeta):
     """
     Metaclass for TaggedObjectNode that maintains a registry
@@ -285,15 +286,15 @@
             self._x_schema = self.get_schema()
         return self._x_schema
 
     def get_schema(self):
         """Retrieve the schema associated with this tag"""
         extension_manager = self.ctx.extension_manager
         tag_def = extension_manager.get_tag_definition(self.tag)
-        schema_uri = tag_def.schema_uri
+        schema_uri = tag_def.schema_uris[0]
         schema = asdfschema.load_schema(schema_uri, resolve_references=True)
         return schema
 
 
 _LIST_NODE_CLASSES_BY_TAG = {}
```

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/testing/assertions.py` & `roman_datamodels-0.9.0/src/roman_datamodels/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/testing/factories.py` & `roman_datamodels-0.9.0/src/roman_datamodels/testing/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,20 @@
     Returns
     -------
     roman_datamodels.stnode.CalStep
     """
     raw = {
         "flat_field": _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
         "dq_init": _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
+        "assign_wcs" : _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
+        "dark" : _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
+        "jump" : _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
+        "linearity" : _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
+        "ramp_fit" : _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
+        "saturation" : _random_choice("N/A", "COMPLETE", "SKIPPED", "INCOMPLETE"),
     }
     raw.update(kwargs)
 
     return stnode.CalStep(raw)
 
 
 def create_coordinates(**kwargs):
```

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/stuserdict.py` & `roman_datamodels-0.9.0/src/roman_datamodels/stuserdict.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/filetype.py` & `roman_datamodels-0.9.0/src/roman_datamodels/filetype.py`

 * *Files identical despite different names*

### Comparing `roman_datamodels-0.8.0/src/roman_datamodels/util.py` & `roman_datamodels-0.9.0/src/roman_datamodels/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """
     # Obtain one of the possible objects the converter returns
     classname = converter_class.types[0]
     # Presume these are from the same directory tree
     rclass = locate(classname)
     tag = rclass._tag
     schema_uri = next(
-        t for t in DATAMODEL_EXTENSIONS[0].tags if t._tag_uri == tag)._schema_uri
+        t for t in DATAMODEL_EXTENSIONS[0].tags if t.tag_uri == tag).schema_uris[0]
     return schema_uri
 
 # def open(init=None, memmap=False, **kwargs):
 #     """
 #     Creates a DataModel from a number of different types
 
 #     Parameters
```

